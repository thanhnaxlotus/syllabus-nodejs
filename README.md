# syllabus-nodejs

## Part 1: Basic JavaScript
### Basic
* [Javascript là gì?](https://freetuts.net/javascript-la-gi-viet-ung-dung-javascript-dau-tien-263.html)
  
  >  Javascript là một ngôn ngữ lập trình kịch bản dựa vào đối tượng phát triển có sẵn hoặc tự định nghĩa. Javascript được sử dụng rộng rãi trong các ứng dụng Website. Javascript được hỗ trợ hầu như trên tất cả các trình duyệt như Firefox, Chrome, ... trên máy tính lẫn điện thoại.

  >  Nhiệm vụ của Javascript là xử lý những đối tượng HTML trên trình duyệt. Nó có thể can thiệp với các hành động như thêm / xóa / sửa các thuộc tính CSS và các thẻ HTML một cách dễ dàng. Hay nói cách khác, Javascript là một ngôn ngữ lập trình trên trình duyệt ở phía client. Tuy nhiên, hiện nay với sự xuất hiện của NodeJS đã giúp cho Javascript có thể làm việc ở backend.
  
  >  Bạn thử truy cập vào một số website trên internet thì sẽ thấy có những hiệu ứng slide, menu xổ xuống, các hình ảnh chạy qua chạy lại rất đẹp. tất cả các chức năng này đều được xử lý bằng Javascript đấy các bạn ạ.
  
  >  Trong những năm gần đây, sự xuất hiện của các framework như NodeJS (chuyên code backend), ExpressJS (NodeJS framework), và nhiều thư viện frontend khác như Angular, jQuery, RactJS ra đời, giúp tạo ra một cơn sốt với từ khóa Javascript Fullstack.


* [Khai báo biến trong Javascript](https://freetuts.net/bien-va-khai-bao-bien-trong-javascript-265.html)

  Có 3 kiểu khai báo biến

  - [ ] `var bar = foo`

  - [x] `const foo = bar`

  - [x] `let zoo = rab`

  > Suggest ticked

* [Các toán tử trong Javascript](https://freetuts.net/cac-toan-tu-trong-javascript-266.html)
  * Toán tử toán học trong javascript
  * Toán tử gán trong javascript
  * Toán tử quan hệ trong Javascript
  * Toán tử luận lý trong Javascript
  * Độ ưu tiên các toán tử trong Javascript
  * Lưu ý với toán tử so sánh bằng Javascript

* [Lệnh if else trong javascript](https://freetuts.net/lenh-kiem-tra-dieu-kien-if-else-trong-javascript-267.html)
* [Lệnh switch case trong Javascript](https://freetuts.net/lenh-switch-case-trong-javascript-402.html)
* [Function trong Javascript](https://freetuts.net/function-trong-javascript-274.html)

```
  const newFn = () => {
    return `Something`
  }
  newFn(); => `Something`
```
```
  function oldFn () {
    return `Something more`
  }
  oldFn(); => `Something more`
```

* Biến toàn cục và cục bộ trong JS

  ```
    // Biến toàn cục
    var comment = "Nội dung comment trước khi thay đổi";
    // Hàm có sử dụng biến toàn cục
    function add_comment()
    {
        comment = "Nội dung comment đa bị thay đổi";
        alert(comment);
    }
    // Gọi fuction comment
    add_comment();
    // In biến toàn cục
    alert(comment);
  ```

* setTimeout và setInterval trong JS
  
  ```
    1. setTimeout
    setTimeout(function(){
        alert("Chào mừng bạn đến với freetuts.net");
    }, 3000);
    var do_alert = function(){
        alert("Chào mừng bạn đến với freetuts.net");
    };
    setTimeout(do_alert, 3000);

    1. clearTimeout
    // hành động
    var action = setTimeout(function(){
        // something
    }, 3000);
    
    // hủy hành động
    clearTimeout(action);

    1. setInterval
    setInterval(function(){
        alert("Chào mừng bạn đến với freetuts.net");
    }, 3000);

    1. clearInterval
    var interval_obj = setInterval(function(){
        alert("Chào mừng bạn đến với freetuts.net");
        clearInterval(interval_obj);
    }, 3000);

  ```
### Loop
* [Vòng lặp for trong Javascript](https://freetuts.net/vong-lap-for-trong-javascript-270.html)
* [Vòng lặp while/do while trong JS](https://freetuts.net/vong-lap-while-do-while-trong-javascript-271.html)
* [Break/Continue trong Javascript](https://freetuts.net/lenh-break-continue-trong-javascript-382.html)

### Data Types
* [String trong Javascript](https://freetuts.net/chuoi-string-trong-javascript-392.html)
* [Hàm xử lý chuỗi trong Javascript](https://freetuts.net/cac-ham-xu-ly-chuoi-trong-javascript-393.html)
* [Mảng trong javascript](https://freetuts.net/thao-tac-voi-mang-trong-javascript-288.html)
* [Các hàm xử lý mảng trong JS](https://freetuts.net/cac-ham-xu-ly-mang-trong-javascript-289.html)
* [Mảng hai chiều trong Javascript](https://freetuts.net/mang-hai-chieu-trong-javascript-3846.html)
* [Number trong Javascript](https://freetuts.net/ham-xu-ly-number-trong-javascript-399.html)
* [Date trong Javascript](https://freetuts.net/doi-tuong-date-trong-javascript-401.html)
* [Xử lý ngày tháng trong Javascript](https://freetuts.net/ham-xu-ly-ngay-thang-date-trong-javascript-400.html)
* [Typeof trong Javascript](https://freetuts.net/ham-typeof-trong-javascript-398.html)

#### Xem Thêm
[Basic JavaScript](https://freetuts.net/javascript-la-gi-viet-ung-dung-javascript-dau-tien-263.html)

## Part 2: Giới thiệu và cài đặt môi trường

* [Cài đặt NodeJS trên Windows](https://phoenixnap.com/kb/install-node-js-npm-on-windows)
* [Cài đặt NodeJS trên Linux - Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-20-04)
* [Cài đặt NodeJS trên MacOS](https://changelog.com/posts/install-node-js-with-homebrew-on-os-x)
* Viết ứng dụng Helloworld với NodeJS

## Part 3: Làm việc với NodeJS

* Node module, module.export và require
* Sử dụng NPM để quản lý package và module trong NodeJS
* File System và làm việc với file trong NodeJS
* Asynchronous và Callback function trong NodeJS
* Asynchronous và cách dùng Promise trong NodeJS
* Tạo webserver cơ bản với HTTP module   
* Tạo Webservice API trả về JSON với HTTP module

## Part 4: Làm việc với ExpressJS Framework

* Cài đặt ExpressJS, xây dựng cấu trúc thư mục cho dự án0
* ExpressJS route
* Cài đặt một số middleware cần thiết: body-passer, session
* Tích hợp Template Engine EJS với ExpressJS
* Cấu hình Static folder JS, CSS, IMAGE

## Part 5: Xây dựng BLOG cá nhân

* Xây dựng giao diện trang chủ Blog
* Route và Logic lấy dữ liệu cho trang chủ
* Xây dựng trang chi tiết bài viết
* Xây dựng trang About cho Blog
