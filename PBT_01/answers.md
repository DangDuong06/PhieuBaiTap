Câu A1:
1.Thứ tự 5 bước xảy ra:
  Bước 1: Request của bạn xuất phát từ laptop đi qua router WiFi nhà trọ.
  Bước 2: Qua nhà mạng VNPT chạy xuyên cáp quang dưới đáy Thái Bình Dương.
  Bước 3: Đến data center của trụ sở Shopee.
  Bước 4: Server Shopee xử lý request (ví dụ: truy xuất các mặt hàng sale, giỏ hàng).
  Bước 5: Response chạy ngược lại (Cáp quang - VNPT - router - laptop); Chrome nhận file HTML, CSS, JS và render ra giao diện trang chủ Shopee.
  Nguồn tham chiếu: tuan_1_html5/01_introduction_html_universe.md - Mục: 🎬 Cuộc Hành Trình 0.3 Giây Xuyên Đại Dương.
2.Trong tab Network khi truy cập shopee:
    Status Code: 200 (yêu cầu thành công)
    Tổng thời gian load lại: 1.49s
    Request CSS: xác định qua cột Type là "Stylesheet"
    *Ảnh minh họa: ![Tab Network Shopee](./screenshots/network_shopee.png)

### Câu A2 — Semantic HTML
**4 lỗi Semantic và cách sửa:**
1. Lỗi: Dùng `<div class="header">` -> Sửa: Thay bằng thẻ `<header>`.
2. Lỗi: Dùng `<div class="menu">` -> Sửa: Thay bằng thẻ `<nav>`.
3. Lỗi: Dùng `<div class="main">` -> Sửa: Thay bằng thẻ `<main>`.
4. Lỗi: Dùng `<div class="footer">` -> Sửa: Thay bằng thẻ <footer>.

### Câu A3 — Block vs Inline
- **Kết quả hiển thị:**
  - "Hộp 1", "Hộp 2", "Hộp 3" mỗi chữ nằm riêng một dòng.
  - "Text A" và "Text B" nằm cùng trên một dòng.
  - "Text C" và "Text D" nằm cùng trên một dòng.
- **Giải thích:** Thẻ `<div>` là phần tử **Block** (chiếm toàn bộ chiều ngang), còn `<span>` và `<strong>` là phần tử **Inline** (chỉ chiếm đủ không gian chứa nội dung).

### Câu A4 — Table
- **Sự khác nhau:**
  - `<thead>`: Phần đầu bảng (tiêu đề).
  - `<tbody>`: Phần thân bảng (chứa dữ liệu).
  - `<tfoot>`: Phần chân bảng (thanh tổng kết/ghi chú).
- **Lý do không dùng table để tạo layout:** 1. Gây khó khăn cho thiết bị đọc màn hình (Accessibility); 2. Làm chậm tốc độ load trang; 3. Khó khăn khi thiết kế Responsive trên Mobile.