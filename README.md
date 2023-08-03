# Làm quen với Unity3D
Làm quen với object 3D + các hàm Move cơ bản

### Phạm vi bài giảng
- Tạo project 3D
- Làm quen với camera : góc nhìn Persp và Iso
- Làm quen với GameObject cơ bản:
  - `Cube`
  - `Sphere`
  - `Capsule`
  - `Cylinder`
  - `Quad`
- Gắn `Rigidbody`(Vật lý) vào GameObject
- Trang trí map với các resource trên `Asset Store`
- Gắn Script vào cho vật thể di chuyển
- Sử dụng DoTween

#### Di chuyển không Rigidbody
| Cách gọi | Mô tả |
| ------ | ------ |
| transform.position = new Vector3(X, Y, Z); | Thay đổi tọa độ của GameObject |
| transform.Translate(X,Y,Z); | Tịnh tiến (dịch chuyển) vị trí của GameObject theo vector(X,Y,Z) |
| transform.position = Vector3.MoveTowards(?); | ??? |
| transform.position = Vector3.Lerp(?); | ??? |
| transform.position = Vector3.SmoothDamp(?); | ??? |

#### Một số method cơ bản
| Cách gọi | Mô tả |
| ------ | ------ |
| if(Input.GetKeyDown(KeyCode.Space)) | Nếu nhấn phím bất kỳ |
| if (Input.GetMouseButtonDown(0)) | Nếu click chuột trái |
| Input.mousePosition | lấy tọa độ chuột |
| Camera.main.transform.position | lấy vị trí camera |

#### Di chuyển với Rigidbody
| Cách gọi | Mô tả |
| ------ | ------ |
| GetComponent<Rigidbody>().velocity = Vector3.right; | Có thể xem như vận tốc |
| GetComponent<Rigidbody>().AddForce(?); | Tác động thêm lực |
