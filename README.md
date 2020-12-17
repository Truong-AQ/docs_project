Docs hướng dẫn kết nối với API

Trong tài liệu này sẽ cung cấp những API của server aigle.blife.ai để có thể lấy được dữ liệu,
hoàn thiện các chức năng của app

Về cơ bản, việc kết nối đến server chúng ta sẽ sử dụng những gói tin http request, sử dụng 2 phương
thức gọi chính là get và post, dữ liệu sẽ được đưa vào header và body (đối với phương thức post) hoặc
params (đối với phương thức get), chúng ta sẽ nhận về những gói tin http, dữ liệu cần thiết có trong phần
header hoặc body của gói tin http response trả về

Tài liệu này sẽ có những thư mục, mỗi thư mục là 1 chức năng của app, bên trong sẽ có các file sau:
- description.txt: miêu tả quá trình gọi các api để thu được kết quả
- các folder, mỗi folder là 1 api, trong mỗi folder chứa các file:
+ file header_response hoặc/và body_response (có thể định dạng html hoặc json), dữ liệu mẫu trả về 
của server mẫu (1 bản tin http response có 2 phần là headers và body)
+ file header_resquest hoặc/và body_request hoặc/và param_request: định dạng các bản tin http được gửi 
đến server và ý nghĩa (1 bản tin http request chung có 2 phần là headers và params và có thể có phần
body nếu phương thức gửi là phương thức post) của các trường
+ file handle.txt: cách điền các trường cần thiết vào request và cách xử lý response trả về từ server

Chức năng của từng folder:
- login: Đăng nhập
- get_test: Lấy các bài kiếm tra của bệnh nhân