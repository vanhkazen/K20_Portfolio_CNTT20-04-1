# Portfolio CV - Trần Việt Anh

Portfolio cá nhân giới thiệu thông tin, kỹ năng, dự án và quá trình học tập của Trần Việt Anh, sinh viên ngành Công nghệ Thông tin. Website tĩnh được xây dựng bằng HTML và CSS; form liên hệ là chức năng thực hành phía trình duyệt, không gửi email hoặc lưu dữ liệu lên máy chủ.

## Liên kết

- **Tác giả:** [Trần Việt Anh](https://github.com/vanhkazen)
- **Hồ sơ GitHub:** https://github.com/vanhkazen
- **Repository:** https://github.com/vanhkazen/K20_Portfolio_CNTT20-04-1
- **GitHub Pages:** https://vanhkazen.github.io/K20_Portfolio_CNTT20-04-1/

> **Trạng thái Pages:** Tại thời điểm viết README, GitHub Pages chưa được bật cho repository (Pages API trả về 404). URL phía trên là địa chỉ dự kiến. Để xuất bản, vào **Settings → Pages**, chọn nhánh `main` và thư mục `/(root)` làm nguồn triển khai; sau khi GitHub hoàn tất deploy, kiểm tra URL Pages ở phần Pages settings.

## Cấu trúc thư mục

```text
.
├── index.html       # Portfolio: giới thiệu, kỹ năng, dự án, học tập, liên hệ
├── ket-qua.html     # Trang đích sau khi gửi form liên hệ
├── css/
│   └── style.css    # Giao diện responsive cho các trang
├── assets/
│   ├── 864870293_1112204684754954_4302107421802050678_n.jpg  # Ảnh đại diện
│   ├── avatar.svg
│   ├── du-an-1.svg
│   ├── du-an-2.svg
│   └── du-an-3.svg
├── AI_LOG.md        # Ghi nhận hỗ trợ AI và sửa lỗi đường dẫn tài nguyên
└── RELEASE_NOTES.md # Ghi chú bàn giao phiên bản v7
```

## Chạy local

Không cần cài thư viện hay build. Từ thư mục gốc của repository, chạy một HTTP server tĩnh:

```bash
python -m http.server 8000
```

Mở [http://localhost:8000](http://localhost:8000) trên trình duyệt. Nếu máy dùng lệnh `python3`, có thể chạy `python3 -m http.server 8000`. Dừng server bằng `Ctrl+C`.

## Kiểm tra trang và chức năng

1. Mở `index.html`; kiểm tra ảnh đại diện, các mục **Giới thiệu**, **Kỹ năng**, **Dự án**, **Học tập**, **Liên hệ** và điều hướng trên đầu trang.
2. Thu nhỏ cửa sổ hoặc mở bằng thiết bị di động để kiểm tra bố cục responsive.
3. Trong phần **Liên hệ**, thử gửi form để trình duyệt kiểm tra các trường bắt buộc, định dạng email, họ tên tối thiểu 2 ký tự và lời nhắn từ 10 đến 500 ký tự.
4. Gửi thông tin hợp lệ để chuyển đến `ket-qua.html`. Form dùng phương thức GET nên dữ liệu sẽ xuất hiện trong URL; không có email nào được gửi và dữ liệu không được lưu trên máy chủ. Không dùng thông tin riêng tư khi thử nghiệm.
5. Từ trang kết quả, dùng **Quay lại liên hệ** hoặc menu để trở lại đúng phần trên trang chính.

## Nguồn xuất bản

Nguồn mã là nhánh `main` của repository. Dự án là website tĩnh, không có bước build hoặc backend; GitHub Pages có thể phục vụ trực tiếp thư mục gốc (`/(root)`) sau khi được bật trong **Settings → Pages**. Các đường dẫn CSS, ảnh và liên kết giữa hai trang đều dùng đường dẫn tương đối để hoạt động trong repository Pages.

## Hồ sơ và minh chứng

- [Hồ sơ cá nhân trên GitHub](https://github.com/vanhkazen)
- [Mã nguồn và lịch sử cập nhật](https://github.com/vanhkazen/K20_Portfolio_CNTT20-04-1)
- [Ghi nhận hỗ trợ AI và các sửa lỗi tài nguyên](AI_LOG.md)
- [Ghi chú bàn giao phiên bản v7](RELEASE_NOTES.md)
