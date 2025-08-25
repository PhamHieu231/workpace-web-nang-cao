PHP Programming
1.1. Giới thiệu về PHP

PHP (Hypertext Preprocessor) là ngôn ngữ lập trình mã nguồn mở, chuyên dùng để viết các ứng dụng web động.

Lịch sử: PHP được tạo ra bởi Rasmus Lerdorf vào năm 1994, ban đầu như một công cụ đơn giản để theo dõi lượt truy cập trên trang cá nhân.

Vì sao chọn PHP?

Dễ học, phổ biến và miễn phí.

Chạy được trên hầu hết các hệ điều hành và web server.

Tích hợp tốt với HTML và cơ sở dữ liệu như MySQL.

PHP là ngôn ngữ server-side: Mã PHP được xử lý trên máy chủ, sau đó kết quả (thường là mã HTML) được trả về trình duyệt người dùng.

1.2. Cú pháp PHP cơ bản

Thẻ PHP:

<?php
    // mã PHP viết ở đây
?>


Biến (Variables):

Bắt đầu bằng ký hiệu $.

Không cần khai báo kiểu dữ liệu trước.

$name = "John";
$age = 25;


Kiểu dữ liệu phổ biến:

Integer (số nguyên)

Float (số thực)

String (chuỗi)

Array (mảng)

Boolean (true/false)

Toán tử:

Số học: +, -, *, /, %

So sánh: ==, !=, >, <, >=, <=

Logic: &&, ||, !

Cú pháp câu lệnh:

Mỗi câu lệnh PHP phải kết thúc bằng dấu ;.

echo "Hello World!";

1.3. Cấu trúc điều khiển

Câu lệnh điều kiện:

if ($age >= 18) {
    echo "Bạn đã đủ tuổi.";
} elseif ($age == 17) {
    echo "Còn 1 năm nữa.";
} else {
    echo "Bạn chưa đủ tuổi.";
}


Vòng lặp:

for: Lặp với số lần xác định.

while: Lặp khi điều kiện đúng.

foreach: Dùng với mảng.

for ($i = 0; $i < 5; $i++) {
    echo $i;
}

1.4. Hàm trong PHP

Định nghĩa hàm:

function sayHello($name) {
    return "Hello, " . $name;
}


Gọi hàm:

echo sayHello("Alice");


Truyền tham số và trả về giá trị:

Có thể truyền nhiều tham số.

Có thể return kết quả để tái sử dụng.

1.5. Vai trò của PHP trong phát triển web

Tạo nội dung động: Giao diện và nội dung thay đổi theo thông tin người dùng hoặc dữ liệu trong database.

Xử lý biểu mẫu:

Nhận và xử lý dữ liệu từ form HTML.

Kiểm tra dữ liệu và phản hồi người dùng.

Tương tác với cơ sở dữ liệu:

PHP thường được dùng với MySQL để lưu trữ, truy xuất và xử lý dữ liệu.

Ví dụ: đăng nhập, đăng ký, lưu bài viết, bình luận, v.v.

Quản lý phiên (Session) và người dùng:

Ghi nhớ trạng thái đăng nhập.

Bảo vệ các trang chỉ cho người dùng đã đăng nhập truy cập.
