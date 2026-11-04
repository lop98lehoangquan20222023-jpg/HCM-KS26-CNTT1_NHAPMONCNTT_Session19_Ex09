# Phần 1:   
1. Tình huống 1:là kết hợp tấn công Phishing và Typosquatting.Chi tiết giả mạo: URL viết sai thành githuh-security.com (sai chữ "hub" thành "huh").
2. Tình huống 2: Là cạm bẫy Mã độc qua phần mềm Crack. Việc yêu cầu tắt Windows Defender nhằm vô hiệu hóa tường lửa/antivirus để mã độc đánh cắp thông tin
3. Áp dụng Quy tắc 5 KHÔNG:

- Tình huống 1: KHÔNG bấm vào liên kết lạ / KHÔNG cung cấp mật khẩu.

- Tình huống 2: KHÔNG tải phần mềm bẻ khóa (crack) / KHÔNG tắt phần mềm bảo vệ.
4. 4 Bước Cấp cứu:

   Ngắt kết nối mạng ngay lập tức.

   Thu hồi quyền truy cập / đăng xuất toàn bộ phiên làm việc.

   Đổi mật khẩu và bật 2FA từ thiết bị sạch.

   Quét sạch mã độc hoặc cài lại hệ điều hành.
# PHẦN 2 – Chuyển sang Password Manager
- Hậu quả khi lộ mật khẩu chung: Hacker dùng mật khẩu đó xâm nhập 2 tài khoản còn lại.
- Zero-Knowledge: Dữ liệu két sắt được mã hóa bằng AES-256 ngay trên thiết bị.Máy chủ Bitwarden hoàn toàn không giữ khóa hay mật khẩu tổng, nên nếu bị hack, chúng cũng không thể giải mã dữ liệu.

Thông số Generator:

Độ dài: 24 đến 32 ký tự

Chữ hoa (A-Z), Chữ thường (a-z), Chữ số (0-9), Ký tự đặc biệt: Bật hết.

# PHẦN 3 – Kích hoạt 2FA cho tài khoản GitHub tổ chức:
1. Lý do dùng Authenticator App (TOTP) thay SMS OTP:Tránh bị tấn công chiếm số điện thoại
2. Các bước kích hoạt trên GitHub:

- Vào Settings -> Password and authentication -> Enable two-factor authentication -> Chọn Authenticator app -> Quét mã QR bằng Google Authenticator -> Nhập mã 6 số để xác nhận.
- Mã khôi phục (Recovery Codes): Nên lưu in ra giấy cất vào két sắt / lưu trong két mật khẩu cá nhân