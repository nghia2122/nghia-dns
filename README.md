# NGHIA DNS — website starter

## Có gì trong gói?
- `index.html`: trang cài đặt DNS mang thương hiệu NGHIA DNS.
- `nghia-dns.mobileconfig`: profile DNS-over-HTTPS cho iPhone/iPad, dùng Cloudflare Public DNS.

## Đưa website lên GitHub Pages
1. Tạo repository mới trên GitHub, ví dụ `nghia-dns`.
2. Giải nén gói ZIP và tải cả `index.html` cùng `nghia-dns.mobileconfig` lên repository (ở thư mục gốc).
3. Vào Settings → Pages.
4. Chọn Deploy from a branch → branch `main` → folder `/ (root)` → Save.
5. Đợi GitHub Pages xuất bản website. Đường dẫn thường có dạng `https://TEN-TAI-KHOAN.github.io/nghia-dns/`.

## Lưu ý quan trọng
- Đây là bản khởi đầu có thể triển khai ngay, không phải bản sao backend của website mẫu.
- Profile đang dùng Cloudflare DoH: https://cloudflare-dns.com/dns-query. Tên NGHIA DNS chỉ là nhãn profile; bạn chưa sở hữu/vận hành DNS resolver riêng.
- Muốn dùng DNS riêng hoặc lọc quảng cáo/domain, cần triển khai resolver và thay endpoint trong profile + website.
- Cấu hình dùng payload `com.apple.dnsSettings.managed`, phù hợp các bản iOS hỗ trợ payload này. Apple đánh dấu payload này deprecated từ iOS/iPadOS 27; nếu thiết bị dùng iOS 27 trở lên, cần kiểm tra phương thức cấu hình DNS mới của Apple trước khi phát hành rộng rãi.
- Không cài profile từ nguồn không tin cậy. Người dùng có thể xem nội dung profile và gỡ nó trong phần quản lý thiết bị của iOS.
