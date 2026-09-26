1. Phân tích lỗi

Lỗi: Dùng lệnh break làm dừng vòng lặp sớm khi gặp món hủy
- Dòng lệnh sai: if (currentDrinkSize === "X") { break; }
- Nguyên nhân: Ký tự 'X' biểu thị ly nước khách hủy tại chỗ. Khi gặp 'X', việc sử dụng lệnh break làm vòng lặp kết thúc ngay lập tức, khiến các ly hợp lệ nằm phía sau (ở đây là ly 'S' và 'M') bị bỏ qua hoàn toàn, dẫn đến thất thoát doanh thu của quán.
- Cách khắc phục: Thay thế lệnh break bằng lệnh continue. Khi gặp 'X', chương trình sẽ bỏ qua ly này và tiếp tục quét các ly hợp lệ tiếp theo trong chuỗi.
