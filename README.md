# Chia Tiền

App chia tiền nhóm. Chạy hoàn toàn trong trình duyệt, không có máy chủ, không gửi dữ liệu đi đâu.

## Đưa lên mạng để gửi link cho bạn bè (GitHub Pages, miễn phí)

1. Tạo repo mới trên GitHub, ví dụ `chia-tien` (để Public).
2. Đẩy nguyên nội dung thư mục này lên nhánh `main`:

   ```bash
   cd chia-tien-app
   git init
   git add .
   git commit -m "Chia Tien PWA"
   git branch -M main
   git remote add origin https://github.com/<ten-github>/chia-tien.git
   git push -u origin main
   ```

3. Vào repo, chọn Settings, Pages, mục Build and deployment chọn
   Source là "Deploy from a branch", Branch là `main`, thư mục `/ (root)`, bấm Save.
4. Chờ 1 đến 2 phút, link có dạng `https://<ten-github>.github.io/chia-tien/`. Gửi link này cho bạn bè.

## Cài như app thật

- iPhone (Safari): mở link, bấm nút Chia sẻ, chọn "Thêm vào Màn hình chính".
- Android (Chrome): mở link, bấm menu ba chấm, chọn "Cài đặt ứng dụng" hoặc "Thêm vào màn hình chính".
- Máy tính (Chrome/Edge): bấm biểu tượng cài đặt ở cuối thanh địa chỉ.

## Lưu ý

- Dữ liệu nằm trong trình duyệt của từng máy. Mỗi người có bảng riêng, đổi máy hoặc xóa dữ liệu trình duyệt sẽ mất.
- Khi sửa code, đổi `VERSION` trong `sw.js` (ví dụ `chia-tien-v2`) để máy người dùng tải bản mới.
- Muốn thử trên máy mình trước: `python3 -m http.server 8000` trong thư mục này rồi mở http://localhost:8000
