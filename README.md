# AZ Coffee Management

Ứng dụng web quản lý cà phê phiên bản MVP, giao diện tiếng Việt, tương thích máy tính và điện thoại.

## Chức năng hiện có
- Dashboard: tổng số lô, tồn kho, mẻ rang, phiếu cupping và hoạt động gần đây.
- Kho cà phê: tạo, tìm kiếm, lọc và xóa lô; quản lý giống, vùng trồng, nhà cung cấp, sơ chế, mùa vụ và khối lượng.
- Rang xay: ghi nhận mẻ rang, đầu vào/đầu ra, nhiệt độ, tính hao hụt và tự động trừ tồn kho.
- Cupping: lưu điểm tổng, người đánh giá, aroma, flavor, acidity/body và ghi chú.
- Truy xuất nguồn gốc: xem thông tin lô và lịch sử rang liên kết.
- Sao lưu: nút **Xuất dữ liệu** tải JSON. Có thể nhấp chuột phải vào nút này để nhập/khôi phục JSON.

## Chạy trên máy tính
1. Giải nén thư mục.
2. Mở `index.html` bằng Chrome, Edge hoặc Firefox.
3. Dữ liệu được lưu trong LocalStorage của trình duyệt đang dùng.

Có thể dùng VS Code và extension Live Server để chạy thuận tiện hơn.

## Đưa lên GitHub Pages
1. Tạo repository mới trên https://github.com (ví dụ `az-coffee-management`).
2. Upload `index.html`, `styles.css`, `app.js`, `README.md` lên nhánh `main`.
3. Vào **Settings → Pages**.
4. Ở **Build and deployment**, chọn **Deploy from a branch**.
5. Chọn branch `main`, folder `/ (root)`, nhấn **Save**.
6. Đợi GitHub Pages xuất bản website và mở URL được cung cấp.

## Lưu ý quan trọng về dữ liệu
Đây là bản MVP chạy phía trình duyệt, chưa có máy chủ hoặc tài khoản người dùng. Dữ liệu chỉ nằm trong trình duyệt và thiết bị hiện tại; xóa dữ liệu trình duyệt hoặc đổi thiết bị có thể làm mất dữ liệu. Hãy xuất JSON sao lưu định kỳ. Không dùng bản này làm hệ thống dữ liệu sản xuất duy nhất.

## Lộ trình nâng cấp đề xuất
- Backend và cơ sở dữ liệu đám mây (ví dụ Supabase/PostgreSQL).
- Đăng nhập, phân quyền chủ cửa hàng / kho / rang / QC.
- Nhật ký nhập-xuất kho, kiểm kê và điều chỉnh tồn có kiểm soát.
- Hồ sơ rang chi tiết: charge temperature, turning point, first crack, drop temperature, development time và roast curve.
- Cupping theo biểu mẫu SCA hoặc biểu mẫu nội bộ; cấu hình thang điểm và thuộc tính.
- QR code cho từng lô, trang truy xuất công khai và báo cáo PDF/Excel.
- Kiểm thử, xác thực dữ liệu, nhật ký thay đổi và sao lưu tự động.

## Cấu trúc
```text
az-coffee-management/
├── index.html
├── styles.css
├── app.js
└── README.md
```
