# Nhật ký sử dụng AI

## Sự cố đường dẫn CSS và hình ảnh

- **Hiện tượng và dữ kiện ban đầu:** CSS không tải; ảnh đại diện và ảnh các dự án không hiển thị. Trong ghi nhận ban đầu, các tài nguyên được mô tả là có trong dự án nhưng đường dẫn chưa đúng. Thư mục `css/` và `assets/` nằm cạnh các trang HTML ở thư mục gốc.
- **Nhận định trước khi hỏi AI:** Tôi nghĩ nguyên nhân có thể là đường dẫn tài nguyên không phù hợp với cấu trúc thư mục hoặc môi trường GitHub Pages; cần kiểm tra tên tệp và đường dẫn tương đối thay vì chỉ dựa vào trạng thái cache của trình duyệt.
- **Công cụ và yêu cầu:** Tôi dùng Copilot AI trong VS Code để hỗ trợ phân tích các ghi nhận “sai đường dẫn css”, “không hiện avatar”, “không hiện ảnh dự án”, rồi đối chiếu đề xuất với cấu trúc và mã nguồn của dự án.
- **Gợi ý từ AI:** Dùng `css/style.css` cho stylesheet; dùng đường dẫn tương đối tới tệp ảnh thực có trong `assets/`; kiểm tra URL tài nguyên và lỗi 404 riêng. AI cũng lưu ý HTTP 304 thường biểu thị tài nguyên được dùng từ cache, không tự nó chứng minh đường dẫn bị lỗi.
- **Quyết định của tôi:** Tôi chọn đường dẫn tương đối vì các tệp nằm trong thư mục con của dự án và cách này phù hợp khi phục vụ website từ thư mục gốc của GitHub Pages. Tôi dùng đúng tên ảnh có trong `assets/`, không đổi tên hay tạo ảnh thay thế. Tôi chưa coi đề xuất của AI là bằng chứng trang đã hiển thị đúng.
- **Phần sửa:** Trong `index.html` và `ket-qua.html`, stylesheet dùng `css/style.css`. Trong `index.html`, ảnh đại diện trỏ tới `assets/864870293_1112204684754954_4302107421802050678_n.jpg`; ảnh dự án trỏ tới `assets/du-an-1.svg`, `assets/du-an-2.svg` và `assets/du-an-3.svg`.
- **Cách thử lại và kết quả đã xác minh:** Kiểm tra cấu trúc tệp và các tham chiếu hiện có trong HTML: những đường dẫn CSS và ảnh nêu trên khớp với tệp trong repository. Có thể thử lại bằng cách chạy `python -m http.server 8000`, mở `http://localhost:8000`, kiểm tra stylesheet và ảnh trên trang chính, rồi xem tab Network của trình duyệt để xác nhận tài nguyên trả về thành công (không phải 404). **Chưa thực hiện kiểm tra hiển thị trên trình duyệt hoặc kiểm tra website đã xuất bản**; GitHub Pages chưa được xác nhận là đã bật.
