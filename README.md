## PHẦN A – COORDINATE SYSTEM & WORLD SPACE 

A1. Tạo một Cube tại vị trí:
X = 2, Y = 1, Z = 5

A2. Bật Gizmos trong Scene View và chụp ảnh thể hiện:

- Trục X

- Trục Y

- Trục Z

A3. Trả lời các câu hỏi:

- Trục nào hướng lên trên trong Unity? => Trục `Y` hướng lên trên trong Unity.
  
- Trục nào hướng về phía Camera? => Trục `Z` (âm) hướng về phía Camera.

<img width="1919" height="1024" alt="Screenshot 2026-01-14 193140" src="https://github.com/user-attachments/assets/fb9e47f4-c0ad-4d66-8817-f8fab2083446" />

## PHẦN B – LEFT-HANDED COORDINATE SYSTEM

B1. Xoay Cube với Rotation:

Y = 90

B2. Quan sát hướng quay của Cube và trả lời:

- Cube quay theo chiều nào? => Quay theo chiều kim đồng hồ ( Khi nhìn từ trên xuống theo trục `Y` ).

- Điều này thể hiện Unity sử dụng Left-Handed Coordinate System như thế nào? => Trong Unity, với trục `Y` hướng lên đối tượng quay theo chiều kim đồng hồ nếu quan sát từ phía trên xuống.

<img width="1919" height="1027" alt="Screenshot 2026-01-14 193555" src="https://github.com/user-attachments/assets/a85cc1cb-e904-47ed-981b-5bde1fd907f6" />

## PHẦN C – LOCAL SPACE VÀ WORLD SPACE

C1. Tạo một Empty GameObject tên là “Parent” tại vị trí:

(5, 0, 0)

C2. Đặt Cube làm con của Parent và thiết lập:

Local Position của Cube = (0, 2, 0)

C3. Ghi lại:

- Local Position của Cube => (0, 2, 0)

<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/8ad6c26f-88a7-4526-95d3-9aebe197a681" />

- World Position của Cube => (5, 2, 0)

<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/c99166f9-86d6-4dfe-87df-30514624f3d7" />

C4. Di chuyển Parent sang vị trí:

(8, 0, 0)

<img width="1919" height="1025" alt="image" src="https://github.com/user-attachments/assets/4d2ea1a6-e91f-4989-bdd4-b594a5cab9ab" />

Trả lời:

- Local Position của Cube có thay đổi không? => Vẫn giữ nguyên (0,2,0).

- World Position của Cube thay đổi như thế nào? => Thay đổi từ (5,2,0) thành (8,2,0).

<img width="1919" height="1024" alt="image" src="https://github.com/user-attachments/assets/3ae6c2ae-d12a-42cf-bee6-86a7d0c5be59" />


