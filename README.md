# App Học Tập – Thi Test (Education App v3.1)

Ứng dụng **học và thi trắc nghiệm** chạy hoàn toàn trên trình duyệt, không cần cài đặt. Phù hợp cho lớp học, cuộc thi tìm hiểu, hoặc tự ôn luyện.

**Demo online:** [https://appluyentap.vercel.app](https://appluyentap.vercel.app)

---

## Tính năng chính

### Dành cho học sinh / người chơi
- **Tự học** – Biết đúng/sai ngay, xem giải thích sau mỗi câu
- **Thi thử** – Làm bài có giới hạn thời gian, chấm điểm cuối bài
- **Phản xạ** – Trả lời nhanh, luyện tốc độ phản ứng
- **Đối kháng** – Thi đấu 2 đội, dùng phím tắt để chọn đáp án
- Lọc câu hỏi theo mức độ (Dễ / Trung bình / Khó) và chủ đề
- Lưu hồ sơ tên + lớp, lịch sử lượt chơi trên trình duyệt

### Dành cho giáo viên / admin
- **Admin Studio** (bảo vệ bằng PIN):
  - Cấu hình tên app, logo, màu sắc, mô tả, thông tin cuộc thi
  - Ngân hàng câu hỏi: thêm / sửa / xóa / xuất bản
  - Quản lý học liệu (IndexedDB)
  - Hỗ trợ AI (Gemini) tạo nội dung / câu hỏi
  - Xem lịch sử làm bài
  - Sao lưu / khôi phục dữ liệu (JSON)

### Kỹ thuật
- Single-file HTML – mở trực tiếp hoặc deploy lên Vercel / GitHub Pages
- Dữ liệu lưu local (localStorage + IndexedDB), không cần server
- Giao diện responsive, hỗ trợ mobile
- Âm thanh phản hồi (có thể tắt)

---

## Cách sử dụng

### 1. Online
Truy cập: [https://appluyentap.vercel.app](https://appluyentap.vercel.app)

### 2. Offline / máy tính
Tải file `index.html` và mở bằng trình duyệt (Chrome, Edge, Firefox…).

### 3. Triển khai riêng
Clone repo và deploy lên Vercel, Netlify hoặc GitHub Pages:

```bash
git clone https://github.com/xaydungnguyenthuc-hub/appluyentap.git
cd appluyentap
```

---

## Cấu trúc

| File | Mô tả |
|------|--------|
| `index.html` | Toàn bộ ứng dụng (HTML + CSS + JS) |

Dữ liệu mặc định gồm bộ câu hỏi về **Nguyễn Văn Trỗi** (tiểu sử, hoạt động cách mạng, mốc lịch sử…). Bạn có thể thay đổi hoàn toàn qua Admin Studio.

---

## Admin

1. Vào trang chủ → nhấn nút **Admin**
2. Nhập PIN (lần đầu có thể đặt PIN trong phần Cấu hình)
3. Quản lý câu hỏi, cấu hình app, xuất/nhập dữ liệu

> **Lưu ý:** PIN chỉ bảo vệ cục bộ trên trình duyệt, không phải hệ thống đăng nhập máy chủ.

---

## Ghi chú

- App chạy hoàn toàn client-side. Xóa dữ liệu trình duyệt sẽ mất hồ sơ, lịch sử và câu hỏi tùy chỉnh (trừ khi đã xuất file sao lưu).
- Phù hợp dùng trong lớp học, cuộc thi tìm hiểu lịch sử / giáo dục, hoặc làm nền tảng quiz tùy chỉnh.

---

## Đóng góp

Nếu phát hiện lỗi hoặc muốn bổ sung tính năng, hãy tạo Issue hoặc Pull Request trên repository này.
