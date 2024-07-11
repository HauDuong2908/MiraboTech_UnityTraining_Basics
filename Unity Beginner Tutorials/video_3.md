# How to make a Video Game in Unity - PROGRAMMING
## 1. Tóm tắt nội dung.
- Tạo Component Script cho Cube(Khối lập Phương).
- Thực hiện trên các Function như Start, Update, FixedUpdate, viết Demo phương thức thêm lực đẩy qua AddForce và Gravity .
- Giải thích về FPS và cách xử lý thông qua Time.deltaTime,
## 2. Nội dung học được.
- Hiểu rõ cách tạo một component Script (name là playerMovement) và thực hiện các hàm sau:
    * Start: Phương thức Start chỉ gọi một lần khi ta bắt đầu Game.
    * Update: Được gọi một lần trên mỗi Frame và được xem như hàm xử lý chính của vòng lặp game, hàm này thực hiện nhiều lần trên mỗi 1 giây.
    * FixedUpdate: Được gọi không phụ thuộc vào vòng lặp chính của Game, mà gọi theo vòng lặp vật lý trong Game
- Hiểu rõ về phương thức viết trong hàm sau:
    * AddForce: giúp ta điều chỉnh về lực đẩy thông qua các trục x, y, z.
    * Time.deltaTime: là thời gian để hiển thị khung hình, được lấy từ thời gian giữa khung hình cuối cùng và khung hình hiện tại.(Lưu ý: khi sử dụng Time.deltaTime thì thông số càng cao thì tốc độ khung hình của giá trị này nhận được sẽ càng thấp).