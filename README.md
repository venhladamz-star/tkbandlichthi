# TKB — Thời Khóa Biểu

Web app xem, chọn và tự chỉnh Thời Khóa Biểu cá nhân từ một nguồn dữ liệu dùng chung. Chạy hoàn toàn trong trình duyệt, không cần cài đặt.

🔗 **App:** https://venhladamz-star.github.io/tkbandlichthi/

## Tính năng

- **Xem TKB dạng lưới** — Thứ 2 đến Thứ 7, Ca 1 đến Ca 4, mỗi ô hiển thị loại tiết (Lý thuyết / Bài tập / Thực hành / Online), phòng học, giảng viên, và ghi chú đặc biệt (vd: "Học từ 16/11").
- **Chọn nhanh theo lớp** — nếu nguồn dữ liệu có mã lớp, chỉ cần chọn đúng lớp là toàn bộ TKB được dựng tự động.
- **Tự ghép TKB riêng** — tick chọn từng môn học phần lẻ để ghép TKB cá nhân, có cảnh báo khi trùng lịch.
- **Tự thêm / sửa môn học** — bấm vào một ô trống hoặc một môn đã có để thêm/sửa trực tiếp. Khi chọn Thứ và Ca, app tự lọc và gợi ý các môn khác đang có sẵn trong nguồn dữ liệu ở đúng khung giờ đó.
- **Xuất ảnh chất lượng cao** — lưu TKB thành ảnh PNG rõ nét, đúng bố cục, dùng để chia sẻ hoặc lưu trữ.
- **Không cần đăng nhập** — TKB cá nhân được lưu ngay trên thiết bị đang dùng.

## Vai trò Admin

Một người quản trị (admin) đăng file TKB tổng (Excel hoặc PDF) làm nguồn dữ liệu dùng chung cho tất cả mọi người — nguồn này được đồng bộ real-time tới mọi thiết bị. Người dùng thường chỉ đọc và chọn từ nguồn đó, không upload hay xóa được nguồn chung, nhưng vẫn tự do thêm/sửa môn học riêng cho TKB của bản thân.

## Công nghệ

- Một file HTML/CSS/JS duy nhất, không cần build.
- [SheetJS](https://sheetjs.com/) để đọc file Excel/CSV, [pdf.js](https://mozilla.github.io/pdf.js/) để đọc PDF.
- [html2canvas](https://html2canvas.hertzen.com/) để xuất ảnh.
- [Firebase Firestore](https://firebase.google.com/products/firestore) để đồng bộ nguồn TKB dùng chung giữa các thiết bị (xác thực ẩn danh, không cần tài khoản).
