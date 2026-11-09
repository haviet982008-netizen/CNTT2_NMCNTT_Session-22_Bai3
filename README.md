1. Báo cáo phân tích theo mô hình IPO
- Input (Đầu vào): Câu trả lời và đoạn mã lệnh sửa lỗi do AI cung cấp.

- Process (Quá trình xử lý & Kiểm chứng):

  1. Sao chép đoạn mã/câu lệnh mà AI cung cấp.

  2. Sử dụng công cụ tìm kiếm với toán tử chuyên sâu (ví dụ: tìm kiếm trên StackOverflow bằng cách dùng site:stackoverflow.com hoặc tra cứu trực tiếp tại tài liệu trang chủ Python) để kiểm tra xem cấu trúc câu lệnh đó có thực sự tồn tại và an toàn không.

  3. Đối chiếu cú pháp xem có lệnh nào can thiệp trái phép vào hệ thống hay phân vùng ổ đĩa hay không (phòng tránh hiện tượng AI Hallucination - AI bịa đặt lệnh sai phiên bản hoặc mã độc hại).

- Output (Đầu ra): Đưa ra kết luận xác nhận lệnh đó là An toàn hay Không an toàn, từ đó quyết định có thực thi hay không.

2. Thiết kế Prompt "hỏi ngược lại" AI để kiểm tra độ an toàn

Hãy phân tích chi tiết câu lệnh bạn vừa cung cấp cho tôi:

  1. Giải thích từng thành phần (tham số, cờ lệnh) trong câu lệnh này có tác dụng gì cụ thể?
 
  2. Câu lệnh này có can thiệp hoặc thay đổi các tệp hệ thống quan trọng (system files/registry) hay không?
  
  3. Cung cấp cho tôi nguồn tài liệu chính thống hoặc link StackOverflow chứng minh đây là cách chuẩn xác để sửa lỗi "Path not found" trên phiên bản hệ điều hành của tôi.
