I.	NỘI DUNG KIỂM THỬ
Kiểm thử chức năng hai nội dung trên website truongnha.com:  Các môn học và Sắp xếp danh sách lớp.
1.	Hướng dẫn chạy
•	Yêu cầu cài đặt
­-	Python 2.7
-­	Robot Framework
­-	Thư viện selenium2library
•	Hướng dẫn chạy
­-	Kiểm thử chức năng Sắp xếp danh sách lớp: file mã nguồn đặt trong thư mục test_listclass. Để chạy kiểm thử ta vào cmd trên địa chỉ chứa thư mục này, gõ “pybot sapxepds.txt”.
­-	Kiểm thử chức năng Sắp xếp, thêm, xóa môn học: file mã nguồn đặt trong thư mục subject/sort_delete_add_subject. Để chạy kiểm thử ta vào cmd trên địa chỉ chứa thư mục này, gõ “pybot sort_subject.txt”.
­-	Kiểm thử chức năng Sửa môn học và thao tác với Chương trình giảng dạy: file mã nguồn đặt trong thư mục subject/content_subject. Để chạy kiểm thử ta vào cmd trên địa chỉ chứa thư mục này, gõ “pybot test_subject.txt”.
Với các nội dung kiểm thử như: sắp xếp, xóa, thêm môn học; sắp xếp danh sách học sinh: cần xác định lại id của môn học, id của học sinh trước khi thực hiện chạy kiểm thử để đảm bảo tồn tại nội dung thực hiện.

2.	Các testcase
	1.		Đăng nhập với đầu vào hợp lệ	Passed
	- Các môn học
	Sắp xếp, thêm, xóa môn học
	2.	Sắp xếp môn học bằng cách sử dụng button Lên/Xuống trên trang web	Passed
	3.		Sắp xếp môn học bằng cách sử dụng các phím mũi tên trên bàn phím	Passed
	4.		Thêm môn học với tất cả các trường hợp lệ	Passed
	5.		Thêm môn học với trường nào đó không hợp lệ	Passed
	6.		Xoá môn học	Passed
	- Sửa môn học, thao tác với Chương trình giảng dạy	
	7.		Sửa môn học với các giá trị hợp lệ	Passed
	8.		Sửa môn học với giá trị nào đó không hợp lệ	Passed
	9.		Xoá hàng nội dung trong chương trình giảng dạy 	Passed
	10.		Sử dụng nội dung chương trình của hệ thống	Passed
	- Sắp xếp danh sách lớp	
	1.		Sắp xếp theo Tên-Họ-Tên đệm 	Passed
	2.		Sắp xếp theo Tên-Tên đệm-Họ	Passed
	3.		Sắp xếp với Kéo thả lên	Passed
	4.		Sắp xếp với Kéo thả xuống	Passed
	5.		Sắp xếp bằng cách trao đổi vị trí của hai học sinh	Passed
II.	NHỮNG KHÓ KHĂN TRONG QUÁ TRÌNH KIỂM THỬ
-	Chỉ sắp xếp môn học bằng button Lên/Xuống với môn học đầu tiên trong trang web.
-	Phần thao tác với chương trình giảng dạy chưa kiểm thử được chức năng thao tác với file bao gồm: Nhập từ Excel và Xuất ra Excel. Do nhóm mới chỉ kiểm thử được đến hiện ra hộp thoại lưu file/tải file lên.
III.	GÓP Ý CHO HỆ THỐNG
-	Phần thêm môn học: có button “Thêm” nhưng không có button “Hủy” thêm môn học, điều này gây khó khăn khi người dùng không muốn hoàn thành việc thêm môn học.
Đề xuất: bổ sung thêm button “Huỷ” bên cạnh button “Thêm”.
-	Phần chỉnh sửa môn học (sau khi click vào tên môn học): phần này sửa đổi, bổ sung cho mỗi môn học: chỉ có button “Lưu” mà không có button “Thoát” nên việc muốn dừng sửa hay quay về trang Các môn học không được thuận tiện.
Đề xuất: bổ sung thêm button “Thoát” bên cạnh button “Lưu”.
-	Hệ thống hiện tại chỉ cho nhập họ và nhập tên, trong trường hợp hai học sinh có tên giống nhau, chẳng hạn, Trần Ngọc Duy mà một trường hợp nhập họ Trần, tên Ngọc Duy; trường hợp kia nhập họ Trần Ngọc, tên Duy thì hai học sinh này mặc dù cùng tên nhưng lại xếp xa nhau trong trường hợp xếp theo Alphabet.
Đề xuất: khi thêm sinh viên, bổ sung thêm trường Tên đệm để nhập tên đệm.
­-	Khi thêm môn học, có thể lọc giáo viên theo chuyên môn được chọn trước để thuận tiện chọn giáo viên phù hợp với môn học được thêm, bởi vì, một giáo viên trung học phổ thông thường chỉ dạy một môn.

