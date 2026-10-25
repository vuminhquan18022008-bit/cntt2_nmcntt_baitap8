# 1 . Phân tích lỗi 
## 1.1 Các lỗi sai của Nam : 
1. Đặt tiêu đề báo cáo chung ngay phía trên tiêu đề cột
2. Chèn dòng tổng hợp vào trong ô dữ liệu có thông tin khác
3. có khoảng trâng ở dòng b4 ở tên Trần Thị Bình
## 1.2 Giải thích : 
Chế độ autofilter chỉ quét dữ liệu chính xác có khoảng trắng ở tên Trần Thị Bình filter sẽ đếm ở vị trí này có thêm 2 kí tự khoảng trắng dẫn đến vô tình k lọc dc thông tin 
# 2. Sửa lỗi 
## 2.1 Cấu trúc bảng chuẩn 

Cột A (STT): Nằm từ A4 (Header: STT) đến A7 (chứa các số thứ tự 1, 2, 3). Không bỏ trống hay chứa chữ tổng hợp.
Cột B (Họ và Tên): Nằm từ B4 (Header: Họ và Tên) đến B7. Toàn bộ dữ liệu trong cột này được làm sạch khoảng trắng thừa bằng công thức =TRIM() (chuyển "Trần Thị Bình  " thành "Trần Thị Bình"). 
Cột C (Khoa / Viện): Nằm từ C4 (Header: Khoa / Viện) đến C7 (chứa tên các khoa như CNTT, Điện tử). Đã xóa bỏ hoàn toàn dòng "TỔNG SỐ CNTT: 45" tại ô C5 cũ để tránh ngắt vùng lọc.   
Cột D (Điểm Xét Duyệt): Nằm từ D4 (Header: Điểm Xét Duyệt) đến D7 (chứa các giá trị số 8.5, 7.9, 8.2). Định dạng đồng nhất dạng Number để phục vụ lọc so sánh $\ge 8.0$.  
Cột E (Trạng Thái): Nằm từ E4 (Header: Trạng Thái) đến E7 (chứa các giá trị Đã duyệt, Chờ duyệt).   
## 2.2 Cách sử dụng đúng hàm Trim 
=TRIM(B5) XONG ĐÓ PASTE VALUES
## 2.2 Cách sử dụng filter 
chọn vào 1 ô bất vkif sau đó tổ hợp phím ctrl + shift + l sau đó click vào dẫu mũi tên để chọn 
