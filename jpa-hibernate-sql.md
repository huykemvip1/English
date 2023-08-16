# Senior
# Transaction
**** Tổng thời gian phản hồi :
	Tổng thời gian lấy kết nối với database 
					+
	Thời gian gửi câu lệnh database qua kết nối 
					+ 
	Thời gian thực hiện câu lệnh đến 
					+ 
	Thời gian trả kết quả 
					+
	thời gian giao dịch không hoại động khi tính toán ở tầng service
	
**** Công thức thông lượng tối đa với số lượng kết nối cơ sở dữ liệu
	
	C(N) = N / 1 + a(N-1) + bN(N-1)
	
	C : là thông lương tương đương chứa được số kết nối cơ sở dữ liệu 
	a : hệ số tranh chấp (phần có thể tuần tự hóa của quy trình xử lý dữ liệu)
	b : hệ số kết hợp (chi phí duy trì tính nhất quán trên tất cả các phiên cơ sở dữ liệu đồng thời)