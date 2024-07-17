# How to make a Video Game in Unity - CAMERA FOLLOW
## 1. Tóm tắt nội dung
- Đưa GameObjet(Camera) vào GameObjet(Player)
- Thực hiện Đưa GameObjet(Camera) kết nối GameObjet(Player) bằng Component Script(FollowPlayer) và viết các phương pháp Hàm sau: 
    * Tạo biến tham chiếu đối với Player thông qua Tranform.
    * Thực hiện phương thức Camera liên kết với vị trí của Player.
    * Thực hiện Vector3 để set lại gốc nhìn Camera so với Player.
## 2. Nội dung học được.
- Cách kết nối MainCamera với GameObject(Player)
- Cách xử lý kết nối tối ưu về MainCamera với GameObject(Player), bằng cách tạo Component FollowPlayer viết phương thức Tranform.position kết nối với Player.position, đồng thời setup lại gốc nhìn của Camera thông Vector3, mục đích để có một cách nhìn cụ thể hơn.