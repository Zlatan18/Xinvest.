# Frame — Studio lên kế hoạch video sản phẩm

Web tiếng Việt, không cần build hoặc API key. Tải ảnh cục bộ, chọn phong cách, tạo storyboard/prompt có thể sửa, sao chép và tải kế hoạch. Đây là công cụ chuẩn bị nội dung; chưa kết nối API tạo video hoặc xuất MP4. Ảnh không được tải lên máy chủ. Thông tin brief được lưu trong localStorage, ảnh chỉ giữ trong phiên.

## Chạy tại máy

```sh
cd /workspace/Xinvest.
python3 -m http.server 8000 --bind 0.0.0.0
```

Mở trình duyệt vào cổng 8000. Không có phụ thuộc cài đặt. Google Fonts là tùy chọn; khi không tải được, trang dùng Arial.

## GitHub Pages

Đưa các tệp lên nhánh `main` của repo `Zlatan18/Xinvest.`. Trong Settings → Pages, chọn Deploy from a branch → main → / (root), rồi Save. Trang dùng đường dẫn tương đối để hỗ trợ tên repo có dấu chấm. Việc xuất bản do chủ kho thực hiện; mã hiện tại không tự đẩy hoặc triển khai.

## Kiểm tra

Kiểm tra tạo kế hoạch 15/20/30 giây, chọn cảnh, sửa prompt, sao chép/tải kế hoạch, tải/xóa ảnh và giao diện di động. Không nhập API key vào mã frontend. Khi bổ sung tạo video trực tiếp, cần backend bảo vệ khóa và xác nhận chi phí trước khi gọi nhà cung cấp.
