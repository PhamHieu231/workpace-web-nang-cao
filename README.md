### 1.1 Giới thiệu PHP 
- PHP viết tắt của Hypertext Preprocessor.
- Là ngôn ngữ lập trình kịch bản chạy phía máy chủ (server-side scripting).
- Được dùng rộng rãi để phát triển web động.

### 1.2 Cú pháp PHP
Mã PHP được đặt trong cặp thẻ như sau:
```
<?php ... ?>
```

Khai báo biến

+ Biến bắt đầu với ký hiệu $, ví dụ: $ten = "phamvhieu";
+ Câu lệnh kết thúc bằng dấu ;

```
$ten = "phamvhieu";
```



Chú thích:

+ Một dòng: // đây là chú thích

+ Nhiều dòng: /* chú thích nhiều dòng */

  ```
  //đây là chú thích một dòng
  /*
   * đây là chú thích nhiều dòng
   */
  
  ```

### 1.3 Cấu trúc điều khiển
PHP hỗ trợ đầy đủ các cấu trúc điều khiển như các ngôn ngữ lập trình phổ biến khác:

#### if .. elseif ...else

Câu lệnh điều kiện: 

```
if ($diem >= 9) {
        echo "Xuất sắc";
    } elseif ($diem >= 7) {
        echo "Khá";
    } else {
        echo "Trung bình";
    }
```
#### Loop : For / while /do...while

Câu lệnh lặp: // for 
```
for ($i = 1; $i <= 5; $i++) {
    echo "Số: $i <br>";
}
```

// while

```

$i = 1;
while ($i <= 5) {
    echo "Số: $i <br>";
    $i++;
}

```

//foreach


```


$mang = array("PHP", "HTML", "CSS");
foreach ($mang as $mon) {
    echo "Môn học: $mon <br>";
}


```


// do...while
```


$i = 0;
do {
  echo $i;
  $i++;
}
while ($i < 5);

```

//Re nhanh switch..case


switch...case: 
```
$ngay = "thu hai";
switch ($ngay)
{ case "thu hai":
  echo "Hôm nay là đầu tuần.";
  break;

  case "thu ba":
  echo "Hôm nay là thứ 3.";
  break;

  default: echo "Không rõ ngày.";
}

```

### 1.4 Hàm trong PHP

+ Giống Methods trong Class
+ Hàm là khối mã thực hiện một nhiệm vụ cụ thể, tái sử dụng.

Ví dụ: 
```
function chao($ten)
{
   return "Xin chào, " . $ten;

}

```

echo chao("Hieu");

Đặc điểm:

+ Có thể có hoặc không tham số.

+ Có thể trả về giá trị bằng return.

PHP cũng hỗ trợ hàm ẩn danh (anonymous functions) và các hàm callback.

### 1.5 Vai trò của PHP trong phát triển ứng dụng Web
PHP giữ vai trò cốt lõi trong lập trình web phía server, cụ thể:

Giúp trang web hiển thị nội dung thay đổi theo từng người dùng hoặc dữ liệu từ cơ sở dữ liệu.

Ví dụ: hiển thị tên người dùng sau khi đăng nhập.

Thu thập dữ liệu từ các form đăng nhập, đăng ký, liên hệ.

Kiểm tra và xử lý dữ liệu trước khi lưu hoặc phản hồi lại.

Kết nối đến MySQL, PostgreSQL…

Thêm, sửa, xóa, tìm kiếm dữ liệu trong bảng.

Ví dụ: lưu thông tin tài khoản, sản phẩm, đơn hàng.

Duy trì trạng thái người dùng giữa nhiều trang (ví dụ: vẫn giữ trạng thái đăng nhập khi chuyển trang).

Quản lý giỏ hàng trong thương mại điện tử.
