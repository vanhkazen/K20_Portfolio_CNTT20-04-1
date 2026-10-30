sai đường dẫn css
không hiện avatar
ko hiện ảnh dự án

## Ghi nhận sửa lỗi

- CSS: dùng đường dẫn tương đối `css/style.css` trong `index.html` và `ket-qua.html`, thay cho đường dẫn Windows không truy cập được trên GitHub Pages.
- Ảnh đại diện: trỏ tới tệp hiện có trong thư mục `assets`.
- Ảnh dự án: thêm tiền tố `assets/` cho các tệp `du-an-1.svg`, `du-an-2.svg` và `du-an-3.svg`.
- Trạng thái: các đường dẫn trên hiện đã được cập nhật trong mã nguồn tại workspace. Cần publish phiên bản này lên GitHub Pages để thay đổi có hiệu lực trên website.
- Ghi chú: HTTP 304 thường có nghĩa là trình duyệt dùng bản cache, không đồng nghĩa tài nguyên bị lỗi; cần kiểm tra URL và trạng thái 404 riêng.
