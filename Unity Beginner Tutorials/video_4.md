# How to make a Video Game in Unity - MOVEMENT
## 1. Tóm tắt nội dung.
- Điều chỉnh RigidBody trong Game Object(player) và tạo component Physiscal Material cho Game Object(Ground)
- Thêm các chức năng mới trong Component Script sau:
    * khởi tạo biến fowardForce và gán giá trị float, mục đích là có thể điều chỉnh lực đẩy trực tiếp trong Unity.
    * khởi tạo slideForce và gán giá trị float, đồng thời gán giá trị Getkey thông qua phương thức điều kiện if vào hàm FixedUpdate, mục đích là khi ta nhấn nút trên Controller thì GameObject(Player) có thể di chuyển trên GameObject(Ground).
## 2. Nội dung học được.
- Hiểu được cách thức điều chỉnh GameObject(Player) thông qua RigidBody.Constrants.FreezeRotation.x, mục đích là làm cho khối lập phương cân bằng so với GameObject(Ground).
- Cách thức tạo Component Physiscal Material và add vào GameObject(Ground), mục đích là tạo độ ma sát với GameObject(player).
- Cách thức tạo biến, Gán giá trị giúp để thay đổi phương thức cố định trong hàm FixedUpdate
- Cách thức viết phương thức câu điều kiện (If) và gán giá Input.Getkey để có thể di chuyển khối lập phương (Cube).