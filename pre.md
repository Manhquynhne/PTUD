1. Xác định yêu cầu
- 3 actors
	+ User (giáo viên):
		- Xem, chỉnh sửa, cập nhật một số thông tin cá nhân
		- Thay đổi password
		- Xem lịch giảng dạy
		- Nhận thông báo từ nhà trường
	+ Trưởng bộ môn:
		- Xem, chỉnh sửa, cập nhật một số thông tin cá nhân
		- Phân bố giáo viên vào từng môn học
		- Thay đổi password
	+ Admin (PTC): 
		- Xem, chỉnh sửa, cập nhật một số thông tin cá nhân
 		- Quản lý giáo viên (tạo, xóa user giáo viên)
		- Phân bố giáo viên vào từng bộ môn
		- Đặt lại mật khẩu cho giáo viên
2. Vẽ use case diagram
Chức năng:
	+ User (giáo viên):
		- Đăng nhập
		- Thay đổi password
		- Chỉnh sửa thông tin cá nhân
		- Xem lịch giảng dạy
		- Nhận thông tin từ nhà trường
	+ Trưởng bộ môn:
		- Đăng nhập
		- Thay đổi password
		- Chỉnh sửa thông tin cá nhân
		- Phân bố giáo viên vào từng môn học
	+ Admin (PTC):
		- Quản lý giáo viên
		- Đọc thông tin giáo viên
		- Đặt lại mật khẩu cho giáo viên
		- Phân bố giáo viên vào từng bộ môn 
3. Thiết kế lược đồ CSDL
	+ USER(uname, pass)
	+ GIAOVIEN(magv, tengv, date, hocham, hocvi, email, sdt, bomon, ngayvaotruong, uname)
	+ LICHDAY(idmonhoc, tenmonhoc, ngay, tiet, ghichu, magv)
	+ TRUONGBOMON(mabomon, magv, tengv, date, hocham, hocvi, email, sdt, bomon, ngayvaotruong) 
	+ THONGBAO(id, tieude, noidung, ngaydang, uname)

4. Thiết kế giao diện
Liệt kê các giao diện web (.html) cần thiết kế
- User (giáo viên): 
+ Đăng nhập: register.html
+ Đăng ký: login.html
+ Trang chủ: index.html (hiển thị thông tin cá nhân (ảnh đại diện, họ tên, bộ môn, mã giáo viên), lịch giảng dạy, thông báo từ nhà trường)
+ Hồ sơ cá nhân: profile.html (hiện thị thông tin( họ tên, mã giáo viên, bộ môn, ngày sinh, email, số điện thoại, học vị, kinh nghiệm), nút chỉnh sửa thông tin)
+ Lịch giảng dạy: schedule.html (hiển thị lịch dạy theo ngày/tuần)
+ Thông báo: notification.html (danh sách thông báo từ nhà trường)
+ Đặt lại mật khẩu: resetpass.html
- Trưởng bộ môn:
	+ Trang chủ: index.html (hiển thị thông tin cá nhân (ảnh đại diện, họ tên, bộ môn, mã giáo viên), lịch giảng dạy, thông báo từ nhà trường, quản lý phân công giáo viên)
	+ Trang phân công môn học: assign_subject.html (phân công giáo viên vào từng môn học)

- Admin (PTC):
	+ Trang chủ: admin_dashboard.html (tổng quan hệ thống)
	+ Quản lý giáo viên: mânge_teachers.html (tạo, xóa, chỉnh sửa thông tin giáo viên)
	+ Quản lý trưởng bộ môn: manage_department_heads.html ( thêm/xóa trưởng bộ môn)
	+ Quản lý bộ môn: manage_department.html (tạo, cập nhật thông tin bộ môn)
	+ Trang phân công bộ môn: assign_department.html ( phân công giáo viên vào bộ môn)
	+ Quản lý thông báo: mange_notification.html
	+ Đặt lại mật khẩu: reset_user_password.html 
