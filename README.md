## PHẦN A – COORDINATE SYSTEM & WORLD SPACE 

A1. Tạo một `Khối` tại vị trí:
X = 2, Y = 1, Z = 5

A2. Bật Gizmos trong Scene View và chụp ảnh thể hiện:

- Trục `X`

- Trục `Y`

- Trục `Z`

A3. Trả lời các câu hỏi:

- Trục nào hướng lên trên trong Unity? => Trục `Y` hướng lên trên trong Unity.
  
- Trục nào hướng về phía `Máy quay`? => Trục `Z` (âm) hướng về phía `Máy quay`.

<img width="1919" height="1024" alt="Screenshot 2026-01-14 193140" src="https://github.com/user-attachments/assets/fb9e47f4-c0ad-4d66-8817-f8fab2083446" />

## PHẦN B – LEFT-HANDED COORDINATE SYSTEM

B1. Xoay `Khối` với `Rotation`:

Y = 90

B2. Quan sát hướng quay của `Khối` và trả lời:

- `Khối` quay theo chiều nào? => Quay theo chiều kim đồng hồ ( Khi nhìn từ trên xuống theo trục `Y` ).

- Điều này thể hiện Unity sử dụng Left-Handed Coordinate System như thế nào? => Trong Unity, với trục `Y` hướng lên đối tượng quay theo chiều kim đồng hồ nếu quan sát từ phía trên xuống.

<img width="1919" height="1027" alt="Screenshot 2026-01-14 193555" src="https://github.com/user-attachments/assets/a85cc1cb-e904-47ed-981b-5bde1fd907f6" />

## PHẦN C – LOCAL SPACE VÀ WORLD SPACE

C1. Tạo một Empty Game`Đối tượng` tên là “Parent” tại vị trí:

(5, 0, 0)

C2. Đặt `Khối` làm con của Parent và thiết lập:

Local Position của `Khối` = (0, 2, 0)

C3. Ghi lại:

- Local Position của `Khối` => (0, 2, 0)

<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/8ad6c26f-88a7-4526-95d3-9aebe197a681" />

- World Position của `Khối` => (5, 2, 0)

<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/c99166f9-86d6-4dfe-87df-30514624f3d7" />

C4. Di chuyển Parent sang vị trí:

(8, 0, 0)

<img width="1919" height="1025" alt="image" src="https://github.com/user-attachments/assets/4d2ea1a6-e91f-4989-bdd4-b594a5cab9ab" />

Trả lời:

- Local Position của `Khối` có thay đổi không? => Vẫn giữ nguyên (0,2,0).

- World Position của `Khối` thay đổi như thế nào? => Thay đổi từ (5,2,0) thành (8,2,0).

<img width="1919" height="1024" alt="image" src="https://github.com/user-attachments/assets/3ae6c2ae-d12a-42cf-bee6-86a7d0c5be59" />

## PHẦN D – GRAPHICS PIPELINE

D1. Di chuyển `Máy quay` dọc trục Z từ -10 đến -3

<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/5faa67ce-c86e-4ca1-904d-ff3175c7dce7" />

<img width="1919" height="1025" alt="image" src="https://github.com/user-attachments/assets/97c80d55-cd77-419b-9382-f07192e6cc16" />

D2. Thay đổi các thông số của `Máy quay`:

- `Phạm vi góc nhìn`: 60 -> 90

<img width="1919" height="1026" alt="image" src="https://github.com/user-attachments/assets/7ef1c1e1-4dde-4777-b2ae-6fad61fbc025" />

- Near Clip Plane: 1 -> 5

<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/b6a11987-d055-480b-9b82-71538211a6c1" />

<img width="1919" height="1029" alt="image" src="https://github.com/user-attachments/assets/a3e72da9-e8d6-4f40-85cb-bcf6c25f1b17" />

Trả lời:

- Vì sao `Đối tượng` trông to hoặc nhỏ hơn dù không đổi vị trí? => Khi `Máy quay` di chuyển lại gần hoặc khi phạm vi góc nhìn giảm, góc nhìn hẹp hơn khiến `Đối tượng` chiếm nhiều diện tích hơn trên màn hình. Ngược lại, khi `Máy quay` lùi xa hoặc `Phạm vi góc nhìn` tăng, `Đối tượng` trông nhỏ hơn dù vị trí của `Đối tượng` không thay đổi.

- Vì sao `Đối tượng` có thể biến mất khỏi màn hình? `Đối tuownjg` có thể biến mất khỏi màn hình khi nằm ngoài vùng hiển thị. Đặc biệt khi `Near Clip Plane` được tăng lên và `Đối tượng` nằm gần `Máy quay` hơn khoảng cách này.

