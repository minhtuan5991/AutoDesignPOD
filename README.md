# AutoMockup Setup

## Cách dùng bộ cài trên máy mới

1. Chép `AutoMockup Setup Lite.exe` sang máy mới.
2. Chạy file bằng quyền người dùng bình thường.
3. Chọn thư mục gốc (Không nên chọn ổ C.). Bộ cài luôn tự tạo thư mục `AutoDesignPOD` bên trong thư mục đã chọn. Ví dụ chọn `F:\AutoEtsy` sẽ cài vào `F:\AutoEtsy\AutoDesignPOD`.
4. Bấm **Cài đặt** để cài bản lõi.
5. Chỉ tích **Cài gói Xóa nền AI local** nếu cần dùng Upscayl + BRIA RMBG 2.0. Gói này có thể tải thêm khoảng 4-5 GB.
6. Đăng nhập Gemini bằng Edge sau khi mở app. (Bắt buộc đăng nhập bằng chức năng đăng nhập trong App để tạo Profile lưu lại tài khoản-Không phải đăng nhập nhiều lần.)

Sau khi cài thành công, bộ cài tự ẩn runtime, source, cấu hình và các file kỹ thuật. Chỉ launcher, `Show technical files.bat` và những thư mục người dùng cần thao tác được để hiện. Chạy `Show technical files.bat` khi cần bảo trì; chạy `Hide technical files.bat` để ẩn lại.

Có thể chạy lại bộ cài vào đúng thư mục cũ để thêm gói Xóa nền AI; file `config.json` và prompt của người dùng được giữ lại.

## Ghi chú

Microsoft Edge và Upscayl là phần mềm bên ngoài. Bộ cài kiểm tra/cài chúng bằng `winget` khi cần. Máy đích cần có Internet trong lần cài đầu tiên; bản Core không cần tải model AI.

## Cập nhật qua GitHub

Trong **Cài đặt > Cập nhật ứng dụng**, nhập repository công khai dạng "ten-tai-khoan/ten-repository" là "minhtuan5991/AutoDesignPOD". Người dùng có thể bấm **Kiểm tra cập nhật** hoặc bật tự động kiểm tra. Updater chỉ thay phần lõi, giữ nguyên runtime/model, `config.json`, profile Edge, prompt, logs và toàn bộ thư mục ảnh. Trước khi thay file, updater xác minh SHA-256 và tạo backup để tự khôi phục nếu có lỗi.
