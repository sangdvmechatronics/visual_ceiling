# Chạy file như sau
Đồng thơif chạy 4 file: v2_main_pro . sub_data_imu. sub_data_all, bdk_test
Thực hiện lấy vị trí từ xla, góc từ imu ban đầu
các hệ số cần chỉnh là dpi_x, dpi_y, kích thước ảnh crop
Hệ số của bđk gồm 3 thông số , hệ số tác động lên x (e[0][0]), y .. , z
Có thể plot tại plot_data để hiển thị định vị, plot_quydaodieukhien để show hết, plot_imu để xem góc tư thế, lưu video, calib ảnh, set ảnh click lấy khoảng cách, 
Có thể sinh quỹ đạo thẳng và tròn tại sinh_quy_dao_thang_tron với cách điều chỉnh như sau:lấy quãng đường chia vận tốc = thời gian chạy, x10 để tìm ra i, cần trừ đi 1 đơn vị để bắt đầu tại vòng lặp tiếp theo, tại quỹ đạo cong thì omega = vận tốc thẳng / bán kính 
tùy theo quay cùng hay ngược kđh mà omega âm hoặc dương, v = omega x bán kính, thời giản chuyển động tròn = góc quay ( giả sử như pi/2 ) chia cho omega x 10 và trừ đi 1 đơn vị
