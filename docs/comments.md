[Home](../README.md)

# Comments

### Line comments (//)

- Dùng để viết comment trên 1 dòng
  Vd: //Line comments

### Block comments (/\*\*/) or Mutiple-line comments

- Có thể sử dụng comment 1 hoặc nhiều dòng.
  Vd: /_Comment trên 1 dòng_/
  /_ Comment trên
  nhiều dòng_/

- Cũng có thể sử dụng ở giữa dòng nếu muốn, điều này có thể làm cho mã của bạn khó đọc hơn.
  Vd: console.log (“Hello” + x /_x is number_/ + “!”);

- Có thể vô hiệu hóa code
  Vd: /_console.log(“Hello”);_/
  !Lưu ý: comment chỉ đóng khi kết thúc bằng (\*/)

### Hashbang comments (#!)

- Hoạt động như line comment (//), ngoại trừ việc bắt đầu bằng (#!) và chỉ hợp lệ khi bắt đầu tuyệt đối của 1 script hoặc module.
- Comment bao gồm tất cả ký tự sau #! cho đến hết dòng đầu tiên.
- Chỉ có 1 comment như vậy được cho phép.
  Vd: #!/usr/bin/env node
  console.log(“Hello”);
   Trình thông dịch Js sẽ coi nó như 1 comment bình thường \_ nó chỉ có ý nghĩa ngữ nghĩa đối với shell nếu tập lệnh được chạy trực tiếp trong shell.
  !Lưu ý: Không được có bất kỳ khoảng trắng nào trước #!
