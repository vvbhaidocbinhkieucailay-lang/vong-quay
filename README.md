# 🎡 Vòng quay chọn thứ tự báo cáo – Chuyên đề Sinh học 10 (HK1)

Trang web nhỏ gọn trong **1 file duy nhất** (`index.html`), không cần cài đặt gì,
không cần mạng mới tải được thư viện (chạy được cả khi mạng trường chậm/chặn CDN).

## Cách chia sẻ cho học sinh

### Cách 1 – Đưa lên GitHub Pages (khuyên dùng, làm 1 lần rồi dùng mãi)

1. Vào [github.com](https://github.com), đăng nhập (chưa có tài khoản thì đăng ký miễn phí).
2. Nhấn dấu **+** ở góc trên phải → **New repository**.
3. Đặt tên repo, ví dụ `vong-quay` → chọn **Public** → nhấn **Create repository**.
4. Trong trang repo vừa tạo, nhấn đường link **uploading an existing file**
   (hoặc nút **Add file → Upload files**) → kéo thả file `index.html` vào → nhấn **Commit changes**.
5. Vào **Settings** (menu trên cùng của repo) → **Pages** (menu trái) →
   mục **Build and deployment** chọn:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` và thư mục `/ (root)` → nhấn **Save**.
6. Chờ 1–2 phút rồi tải lại trang, GitHub hiện link dạng:

   ```
   https://<tên-tài-khoản>.github.io/vong-quay/
   ```

7. Copy link đó gửi vào nhóm Zalo / Google Classroom cho học sinh.
   Học sinh mở link trên điện thoại là quay được ngay.

> Lần sau muốn sửa danh sách nhóm: sửa file `index.html` (xem mục bên dưới),
> upload đè file cũ trong repo là link tự cập nhật.

### Cách 2 – Gửi thẳng file

Gửi file `index.html` qua Zalo/email. Người nhận tải về và mở bằng Chrome.
Lưu ý: trên iPhone việc mở file HTML khá bất tiện, nên vẫn khuyên dùng **Cách 1**.

## Đổi tên nhóm / số lượng nhóm

Mở `index.html` bằng Notepad (hoặc bất kỳ trình soạn thảo nào), tìm đến dòng:

```js
const DANH_SACH_NHOM = [
    "Nhóm 1", "Nhóm 2", ... "Nhóm 8"
];
```

Sửa tên hoặc thêm/bớt nhóm cho đúng lớp, lưu lại là xong. Có thể đổi cả dòng
`TEN_BAI` (tên bài hiển thị trong tin nhắn chia sẻ kết quả).

## Tính năng

- Quay ngẫu nhiên công bằng — mỗi nhóm chỉ được chọn đúng 1 lần.
- **Tự lưu kết quả** trên từng máy (tải lại trang không mất), nút **Làm mới** để quay lại từ đầu.
- Nút **📤 Chia sẻ kết quả**: tạo sẵn tin nhắn thứ tự báo cáo — trên điện thoại
  mở thẳng bảng chia sẻ của Zalo/Messenger để gửi vào nhóm lớp; trên máy tính thì copy.
- Nút **⬇ Tải CSV**: mở bằng Excel, có sẵn cột *Tên thành viên, Điểm chấm chéo, Điểm báo cáo lần 1* để chấm điểm.
- Âm thanh "tạch tạch" khi quay + nhạc chúc mừng (có nút tắt tiếng), hiệu ứng pháo giấy.
- Nhấn **Space** để quay khi trình chiếu máy chiếu.
