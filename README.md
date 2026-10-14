Atlas Thần Kinh 3D — bản web có khóa
© 2026 Lê Hữu Sơn Hải & Phạm Tuấn Kiệt. Bảo lưu mọi quyền. Xem NOTICE.md.

Đưa lên mạng: tải cả thư mục này lên một host tĩnh bất kỳ, ví dụ:
  - GitHub Pages: tạo repo, đưa các tệp vào, bật Settings → Pages;
  - Netlify: kéo thả thư mục vào app.netlify.com/drop;
  - host của trường.
Mở trực tiếp index.html trên máy cũng chạy được.

Người xem phải nhập key truy cập. Toàn bộ nội dung được mã hóa AES-256-GCM trong app.enc.js;
không có key thì không đọc được, kể cả khi tải các tệp về.

Đổi key: chạy lại  python tools/build_locked.py --key "KEY-MỚI"  rồi tải lại thư mục site/.
Nhiều key, key có hạn:  --key "KEY-MỚI" --key "KEY-CŨ@2026-10-17"  (key cũ hết hạn 23:59 ngày đó, giờ Việt Nam).
Key hết hạn bị trang từ chối ngay; tác vụ .github/workflows/prune-expired-keys.yml (GitHub Actions) gỡ hẳn
key hết hạn khỏi app.enc.js mỗi ngày.
Liên kết mở sẵn (chỉ gửi cho người tin cậy):  <địa chỉ>/#k=KEY
