### 1. Tại sao truy vấn trên là "Bad Query" (gây nhiễu)?

Câu truy vấn *"thầy ơi cho em xin tài liệu học html cơ bản của trang mozilla với ạ"* bị đánh giá là một **Bad Query** vì các nguyên nhân sau:

* **Sử dụng văn phong giao tiếp thừa thãi:** Các cụm từ như *"thầy ơi"*, *"cho em xin"*, *"của trang"*, *"với ạ"* là ngôn ngữ hội thoại dành cho con người, không phải từ khóa kỹ thuật. Việc đưa vào công cụ tìm kiếm làm loãng trọng tâm truy vấn.
* **Không khoanh vùng tên miền gốc:** Chỉ ghi chữ *"mozilla"* chung chung khiến Google hiểu đây là một từ khóa nội dung thông thường. Kết quả trả về sẽ bao gồm vô số trang web bên thứ ba chỉ nhắc đến từ "Mozilla" thay vì trang tài liệu chính thức của hãng (`developer.mozilla.org`).
* **Dễ kích hoạt các kết quả quảng cáo và SEO rác:** Cụm từ *"tài liệu học html cơ bản"* trùng khớp với từ khóa quảng cáo của nhiều trung tâm đào tạo, trang bán khóa học và các diễn đàn hỏi đáp không liên quan.

### 2. Viết lại truy vấn tối ưu sử dụng toán tử `site:` và `-`

Để tìm đúng tài liệu gốc của Mozilla (MDN Web Docs) và loại bỏ nội dung rác, sinh viên nên viết lại truy vấn theo một trong hai cách sau:

* **Truy vấn tìm tài liệu tiếng Việt trên MDN:**
  ```text
  site:developer.mozilla.org HTML cơ bản -khóa-học -quảng-cáo -diễn-đàn
  ```

* **Truy vấn tìm tài liệu gốc tiếng Anh chuẩn trên MDN (khuyên dùng):**
  ```text
  site:developer.mozilla.org "HTML basics" -course -ads -forum
  ```

### 3. Ý nghĩa của các toán tử trong việc tiết kiệm thời gian lọc tin

* **Toán tử `site:developer.mozilla.org` (Khoanh vùng nguồn uy tín):** Ép bộ máy tìm kiếm của Google chỉ trả về các trang nằm trong hệ thống tài liệu kỹ thuật chính thức của Mozilla (MDN Web Docs). Điều này loại bỏ hoàn toàn các blog tổng hợp, trang tin rao vặt hoặc nguồn kiến thức sai lệch.
* **Toán tử `-` (Loại trừ từ khóa rác):** Gắn dấu trừ liền trước từ khóa (như `-khóa-học`, `-quảng-cáo`, `-diễn-đàn`) giúp chặn đứng các trang chứa nội dung thương mại, mời chào đăng ký học hoặc các luồng thảo luận lan man không đi vào trọng tâm.
* **Hiệu quả tiết kiệm thời gian:** Thay vì phải mở hàng chục tab và tự đọc để sàng lọc giữa hàng triệu kết quả hỗn tạp, người dùng nhận được ngay đường dẫn tài liệu chuẩn xác nhất ngay ở vị trí đầu tiên trên trang kết quả tìm kiếm.
