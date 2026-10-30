# Release notes - Portfolio CV v7

- **Tên sản phẩm:** Portfolio CV - Trần Việt Anh
- **Phiên bản bàn giao:** v7
- **Ngày cập nhật:** 2026-10-30
- **Tác giả:** Trần Việt Anh

## Thay đổi chính

- Hoàn thiện portfolio tĩnh bằng HTML và CSS, gồm các phần giới thiệu, kỹ năng, dự án, học tập và liên hệ.
- Bổ sung trang kết quả cho form liên hệ và bố cục responsive.
- Chuẩn hóa đường dẫn CSS và hình ảnh theo thư mục `css/` và `assets/` để dùng đường dẫn tương đối trong dự án.
- Bổ sung hướng dẫn sử dụng trong [README.md](./README.md) và ghi nhận quá trình hỗ trợ AI trong [AI_LOG.md](./AI_LOG.md).

## Lỗi đã sửa

- Sửa tham chiếu stylesheet để tải `css/style.css` trên cả trang chính và trang kết quả.
- Sửa đường dẫn ảnh đại diện và ba ảnh dự án để tham chiếu đúng các tệp trong `assets/`.

## Mã nguồn và commit liên quan

Repository: [vanhkazen/K20_Portfolio_CNTT20-04-1](https://github.com/vanhkazen/K20_Portfolio_CNTT20-04-1).

Mốc mã nguồn gần nhất có trong lịch sử Git là commit [`aeb6197`](https://github.com/vanhkazen/K20_Portfolio_CNTT20-04-1/commit/aeb6197ff66b16ae0f6ea2b0076b3b6c9c78cd3f) trên nhánh `main`. Xem [cây mã nguồn tại commit này](https://github.com/vanhkazen/K20_Portfolio_CNTT20-04-1/tree/aeb6197ff66b16ae0f6ea2b0076b3b6c9c78cd3f), bao gồm [index.html](https://github.com/vanhkazen/K20_Portfolio_CNTT20-04-1/blob/aeb6197ff66b16ae0f6ea2b0076b3b6c9c78cd3f/index.html), [ket-qua.html](https://github.com/vanhkazen/K20_Portfolio_CNTT20-04-1/blob/aeb6197ff66b16ae0f6ea2b0076b3b6c9c78cd3f/ket-qua.html), [css/style.css](https://github.com/vanhkazen/K20_Portfolio_CNTT20-04-1/blob/aeb6197ff66b16ae0f6ea2b0076b3b6c9c78cd3f/css/style.css) và thư mục [assets](https://github.com/vanhkazen/K20_Portfolio_CNTT20-04-1/tree/aeb6197ff66b16ae0f6ea2b0076b3b6c9c78cd3f/assets).

**Lưu ý về bàn giao:** v7 là nhãn phiên bản cho đợt bàn giao này; repository chưa có tag v7. Khi lập ghi chú này, `README.md`, `AI_LOG.md` và `RELEASE_NOTES.md` đang có thay đổi trong working tree chưa được commit. Vì vậy, permalink commit phía trên trỏ tới mốc mã nguồn đã commit, không bao gồm các cập nhật tài liệu chưa commit này. Muốn phát hành một snapshot v7 duy nhất, hãy commit các tệp bàn giao rồi cập nhật liên kết tới commit mới.

## Hạn chế còn lại

- GitHub Pages chưa được xác nhận đã bật; URL trong README là địa chỉ dự kiến cho đến khi kiểm tra deployment trong repository settings.
- Form dùng GET để thực hành kiểm tra HTML5, không gửi email và không lưu dữ liệu. Giá trị gửi có thể xuất hiện trong URL; chỉ dùng dữ liệu thử không nhạy cảm.
- Liên kết GitHub ở các thẻ dự án trong trang hiện là nội dung chờ cập nhật, chưa phải liên kết tới repository dự án thực tế.
- Chưa xác minh trực quan website trên trình duyệt hoặc trên GitHub Pages cho bản bàn giao này.

## Tiếp tục kiểm tra và bàn giao

1. Chạy `python -m http.server 8000` ở thư mục gốc rồi mở `http://localhost:8000`.
2. Kiểm tra CSS, ảnh đại diện, ảnh dự án, điều hướng, bố cục ở màn hình hẹp, xác thực form và chuyển tiếp tới `ket-qua.html`. Có thể xem tab Network để xác nhận tài nguyên không trả về 404.
3. Trong **Settings → Pages**, chọn nhánh `main` và thư mục `/(root)`; sau khi deploy, xác nhận URL Pages thực tế và kiểm tra cả hai trang trên URL đó.
4. Cập nhật các liên kết dự án đang chờ nếu đã có repository tương ứng; không dùng dữ liệu cá nhân thật khi thử form GET.
5. Commit snapshot v7 và thay permalink ở mục **Mã nguồn và commit liên quan** bằng commit bàn giao cuối cùng.