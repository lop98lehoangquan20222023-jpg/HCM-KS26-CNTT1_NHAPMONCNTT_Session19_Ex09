# PHẦN 1: BÁO CÁO PHÂN TÍCH KIẾN TRÚC AN NINH
1. Rủi ro khi lưu mật khẩu trên Chrome (Login Data):

- Mật khẩu bị lưu ở dạng mã hóa yếu.

- Khi dính mã độc Infostealer, hacker dễ dàng lấy file dữ liệu này và giải mã ngay lập tức trên máy của bạn mà không cần biết mật khẩu tổng, đồng thời đánh cắp luôn phiên đăng nhập để vượt qua 2FA.

2. Kiến trúc Zero-Knowledge & Client-side Decryption:

- Dữ liệu được mã hóa hoàn toàn bằng AES-256 ngay trên thiết bị của bạn (Client) trước khi gửi lên đám mây.

- Nếu máy chủ Bitwarden bị hack? Hacker không thể giải mã dữ liệu vì máy chủ hoàn toàn không giữ khóa hay mật khẩu tổng (Zero-Knowledge).

# PHẦN 2: THIẾT KẾ CHÍNH SÁCH & KỊCH BẢN CHUYỂN ĐỔI
3. Tạo Master Passphrase đạt chuẩn:

Nguyên tắc: Dài tối thiểu 20 ký tự, kết hợp từ ngẫu nhiên, số và ký tự đặc biệt để chống tấn công vét cạn.

Ví dụ: Tieu-Hổ-Bay-Giữa-Mây-99!$2026

4. Cấu hình Generator trong Bitwarden cho 40 tài khoản:

Loại: Password | Độ dài: 24 - 32 ký tự

Tích chọn đầy đủ: Chữ hoa (A-Z), Chữ thường (a-z), Số (0-9), và Ký tự đặc biệt (!@#$).

5. Auto-fill chống Phishing tốt hơn con người:

Bitwarden chỉ tự động điền khi tên miền khớp chính xác 100% với dữ liệu đã lưu. Các trang web lừa đảo giả mạo tên miền (ví dụ: githúb.com) sẽ bị từ chối điền, giúp cảnh báo người dùng ngay lập tức.

