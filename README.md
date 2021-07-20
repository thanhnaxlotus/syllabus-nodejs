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
  * setTimeout
  setTimeout(function(){
      alert("Chào mừng bạn đến với freetuts.net");
  }, 3000);
  var do_alert = function(){
      alert("Chào mừng bạn đến với freetuts.net");
  };
  setTimeout(do_alert, 3000);

  * clearTimeout
  // hành động
  var action = setTimeout(function(){
      // something
  }, 3000);
  
  // hủy hành động
  clearTimeout(action);

  * setInterval
  setInterval(function(){
      alert("Chào mừng bạn đến với freetuts.net");
  }, 3000);

  * clearInterval
  var interval_obj = setInterval(function(){
      alert("Chào mừng bạn đến với freetuts.net");
      clearInterval(interval_obj);
  }, 3000);

```
### Loop
* [Vòng lặp for trong Javascript](https://freetuts.net/vong-lap-for-trong-javascript-270.html)

`EXERCISE:` 
> Dùng for hiển thị đầu ra bằng console.log
```
var domains = [
    'freetuts.net',
    'qa.freetuts.net'
];
```

* [Vòng lặp while/do while trong JS](https://freetuts.net/vong-lap-while-do-while-trong-javascript-271.html)

`EXERCISE:` 
> Đầu ra của đoạn code bên dưới là gì?
```
while (i < 10) {
  console.log(`The number is ${i}`)
  i++;
}
```

* [Break/Continue trong Javascript](https://freetuts.net/lenh-break-continue-trong-javascript-382.html)

`EXERCISE:` 
> Đầu ra của đoạn code bên dưới là gì?
```
for (var i = 0; i < 10; i++){
    console.log(i);
}
```

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

## Part 2: Giới thiệu và cài đặt môi trường

* [Cài đặt NodeJS trên Windows](https://phoenixnap.com/kb/install-node-js-npm-on-windows)
* [Cài đặt NodeJS trên Linux - Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-20-04)
* [Cài đặt NodeJS trên MacOS](https://changelog.com/posts/install-node-js-with-homebrew-on-os-x)

## Part 3: Làm việc với NodeJS
* [Package `node-persist` - Local Storage trên Server](https://freetuts.net/node-persist-local-storage-tren-server-589.html)

> Để lưu trữ dữ liệu tạm thời thì trong Javascript HTML5 có khái niệm `LocalStorage` và `SessionStorage`, còn trong PHP thì có khái niệm session. Vậy trong NodeJS có cách nào để lưu trữ dữ liệu tạm thời hay không? Có đấy các bạn, chúng ta sẽ sử dụng module `node-persist` để lưu trữ dữ liệu tạm thời trên Server (không lưu trong hệ quản trị CSDL mà lưu file và bộ nhớ).

`EXERCISE:`
> Xây dựng 1 mini app CRUD quản lý học sinh hoặc sinh viên biểu diễn dưới dạng Class và sử dụng `node-persist` để lưu trữ dữ liệu.

* [Node module, module.export và require](https://viblo.asia/p/nodejs-require-exports-and-moduleexports-djeZ18PQKWz)
* [Asynchronous và Callback function trong NodeJS](https://viblo.asia/p/tim-hieu-ve-vong-lap-callback-promise-va-asyncawait-trong-javascript-Do754ekXKM6)
* [Asynchronous Promise vs Async/Await trong NodeJS](https://ehkoo.com/bai-viet/tat-tan-tat-ve-promise-va-async-await)

## Part 4: MODULE

* [Module Path trong NodeJS](https://freetuts.net/module-path-trong-nodejs-672.html)
* [Module URL trong NodeJS](https://freetuts.net/module-url-trong-nodejs-673.html)
* [Module FS trong NodeJS](https://freetuts.net/module-fs-trong-nodejs-674.html)

## Part 5: Server

* [Callback trong NodeJS](https://freetuts.net/callback-trong-nodejs-2184.html)
* [Events trong NodeJS](https://freetuts.net/events-trong-nodejs-2186.html)
* [Buffer trong NodeJS](https://freetuts.net/buffer-trong-nodejs-2194.html)
* [Streams trong NodeJS](https://freetuts.net/streams-trong-nodejs-2202.html)
* [HTTP Web Server trong Nodejs](https://freetuts.net/khoi-tao-http-web-server-trong-nodejs-2214.html)
* [NodeJS Server đơn giản](https://freetuts.net/xay-dung-nodejs-server-don-gian-666.html)
* [writeHead + setHeader NodeJS](https://freetuts.net/ham-writehead-va-setheader-trong-nodejs-671.html)
* [process.env trong Nodejs](https://freetuts.net/process-env-nodejs-2228.html)
* [Upload files trong Nodejs](https://freetuts.net/upload-files-trong-nodejs-2223.html)
* [Xử lý CORS trong NodeJS](https://freetuts.net/cors-la-gi-xu-ly-cors-trong-nodejs-2730.html)

## Part 6: Mongo

* [MongoDB trong NodeJS](https://freetuts.net/gioi-thieu-mongodb-trong-nodejs-2294.html)
* [Kết nối với MongoDB](https://freetuts.net/ket-noi-voi-mongodb-trong-nodejs-2296.html)
* [Mongoose trong NodeJS](https://freetuts.net/mongoose-trong-nodejs-2307.html)
* [Schemas trong Mongoose](https://freetuts.net/schemas-trong-mongoose-2308.html)
* [SchemaTypes trong Mongoose](https://freetuts.net/schematypes-trong-mongoose-2315.html)
* [Models trong Mongoose](https://freetuts.net/models-trong-mongoose-2316.html)
* [Documents trong Mongoose](https://freetuts.net/documents-trong-mongoose-2317.html)
* [Subdocuments trong Mongooose](https://freetuts.net/subdocuments-trong-mongooose-2319.html)
* [CRUD trong Mongoose](https://freetuts.net/create-read-update-delete-trong-mongoose-2321.html)
* [Validation trong Mongoose](https://freetuts.net/validation-trong-mongoose-2322.html)
* [Middleware trong Mongoose](https://freetuts.net/middleware-trong-mongoose-2323.html)
* [Populate trong Mongoose](https://freetuts.net/populate-trong-mongoose-2332.html)

## Part 7: Xây dựng BLOG cá nhân

* [BASE PROJECT](https://github.com/thanhnaxlotus/ltsxnode)

`SUGGESTION:`
1. Clone base project được gắn link ở trên
2. Chạy nó lên và cài template engine bạn muốn sử dụng. Vd: [ejs](https://ejs.co/), [handlebarsjs](https://handlebarsjs.com/), ...

`REQUIREMENT:`

* Xây dựng giao diện trang chủ Blog
* Route và Logic lấy dữ liệu cho trang chủ
* Xây dựng trang chi tiết bài viết
* Xây dựng trang About cho Blog

## Part 8: Xây dựng 1 trang web bán hàng bằng nodejs

`REQUIREMENT:`

* Site quản trị
* Site bán hàng