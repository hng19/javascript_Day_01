# Javascript Cơ bản

## Khái niệm về biến
Biến là một định danh dùng để lưu trữ dữ liệu, thông qua biến chúng ta có thể thực hiện các thao tác với dữ liệu.

Mỗi biến có một kiểu dữ liệu riêng, dựa vào kiểu dữ liệu của biến có các thao tác khác nhau với biến.

## Khai báo biến
Để khai báo biến sử dụng từ khóa : let / const.
Sử dụng 2 cách sau để khai báo biến:
* Khai báo biến và không gán giá trị cho biến: let name;
* Khai báo biến và gán giá trị cho biến: let name = 1;

VD:
```js
 // Khai báo biến
let name = ok;
console.log(name);

//gán giá trị cho biến
let name="Hoàng Hồng";
console.log(name);

//c1 vừa khai báo biến vừa gán giá trị cho biến
let email="hoangvanhong142@gmail.com";
console.log(email);

//Khai báo biến sử dụng const
const pi=3.14;
console.log(pi);

//Khai báo chuỗi rỗng
let emptyString = "";
```
> *Chú ý: 
khi một biến chưa gán giá trị sẽ nhận giá trị là undefinedsss*

## Quy tắc đạt biến
* Chứa các kí tự chữ, số, _ và $.
* Ký tự đầu tiên không được là số(nên là chữ).
* Có phân biệt chữ hoa hay chư thường.
* Không trùng các từ khóa trong Javascipt như: for, while, this,[...](http://https://www.w3schools.com/js/js_reserved.asp?gidzl=QXVcJjrvsZfc3-T0tMFUF683u4V3OuuzBGEm4v5jX6mc1Rv3pp-BFNa2iqUKQOSzVLBlGZQFM0nCrtlUCG)
* Nên đặt tên theo kiểu **camelCase** nếu tên biến có độ dài 2 từ trở lên cho dễ đọc. VD: **fullname** thì nên đặt là **fullName**.
## Kiểm tra dữ liệu của biến
Sử dụng **typeof**
```js
let n = 1
console.log(typeof n)//  xuất ra kết quả ;là "number"

let name = "Hoàng Hồng"
console.log(typeof name)// xuất ra kết quả là "string"
```
## Kiểu dữ liệu String
String (chuỗi) là một đoạn text có thể có một hoặc nhiều ký tự.

Các chuỗi đều phải được bao quanh bằng cặp dấu nháy đơn `’` hoặc nháy kép `"` hoặc dấu "backtick" ( ` ).
## Một số lưu ý
Trường hợp trong chuỗi cũng có xuất hiện dấu nháy đơn hoặc nháy kép thì phải thêm ký tự `\` đằng trước dấu nháy đó.

```js
let message = "Xin chào các bạn, mình tên là \"Hoàng Hồng\". Mình sinh năm 2003";
```

Khi bạn muốn Enter xuống hàng một chuỗi thì bắt buộc phải sử dụng dấu `+` để nối chuỗi.

```js
let message = "Xin chào các bạn, " +
"mình tên là \"Hoàng Hồng\". " +
"Mình sinh năm 2003";
```

## Kiểu của null

Kiểu dữ liệu **null** là một kiểu dữ liệu đặc biệt, chỉ bao gồm một giá trị là `null` (`null = 0`), VD:

```js
let language = null;
console.log(language); // null
```
> Chú ý:
Khác nhau cơ bản giữa **undefined** và **null**:
Kiểu dữ liệu **null** là kiểu dữ liệu được gán cho biến, thường được hiểu là **không biết** (không có).
Trong khi đó, kiểu dữ liệu **undefined** là giá trị mặc định của biến sau khi khai báo mà **không gán giá trị** cho biến.

## Kiểu dữ liệu Boolean (Kiểu Logic)

Boolean là kiểu dữ liệu logic chỉ bao gồm hai giá trị là `true` (đúng, chính xác, `true = 1`) và `false` (sai, không chính xác, `false = 0` ), VD:

```js
let isWebLoaded = true; // => Trang web đã được tải xong
console.log(isWebLoaded); // true

let isProgramRunning = false; // Chương trình đang không chạy
console.log(isProgramRunning); // false
```

## Nối chuỗi trong Javascript

Để nối chuỗi chúng ta sử dụng dấu `+` để ghép hai chuỗi (hoặc biến) lại với nhau.

```js
//Cộng chuỗi
let firstName = "Hoàng";
let lastName = "Hồng";

let fullName = firstName + " " + lastName;
console.log(fullName)
```

## Template Strings
Sử dụng cú pháp với "back-tick"
`string_text ${expression} string_text`
VD:
```js
//sử dụng Template string
let name = "Hoàng Hồng"
let year = 2003 
let message =`Xin chào các bạn, mình tên là "${name}" , mình sinh năm ${year}. Năm nay mình ${2022 - year} tuổi`;
console.log(message);
```


## Kiểu dữ liệu number

JavaScript có hai loại số là: **số nguyên** và **số thực**.
```js
let n1 = 66; // số nguyên dương
let n2 = -66; // số nguyên âm
let n3 = 3.14; // số thực dương
let n4 = -3.14; // số thực âm
let n5 = 2e3; // => 2*10^3 = 2000
let n6 = 2e-3; // => 2*10^(-3) = 0.002
let n7 = 0xff; // số dạng hexa (hệ cơ số 16): 15*16 + 15 = 255
let n8 = 067; // số dạng octa (hệ cơ số 8): 6*8 + 7 = 55
let n9 = 0b11; // số dạng nhị phân (hệ cơ số 2): 1*2 + 1 = 3
```
Ngoài những loại số trên, JavaScript còn có 3 số đặc biệt là: Infinity, -Infinity và NaN.

*Infinity: là số dương vô cùng.

```js
console.log(Infinity); // Infinity
console.log(1 / 0); // Infinity
```
-Infinity: là số âm vô cùng.

```js
console.log(-Infinity); // -Infinity
console.log(-1 / 0); // -Infinity
```

NaN: là viết tắt của Not a Number.
```js
// Lấy 0 / 0
console.log(0 / 0); // NaN

// Lấy chuỗi ký tự chia cho số
console.log("JavaScript" / 2); // NaN

// Lấy hai số Infinity trừ cho nhau
console.log(Infinity - Infinity); // NaN
```

## Sử dụng `Math` trong Javascript
```js
// Math.PI : số pi
console.log(Math.PI); // 3.141592653589793
```
### Làm tròn
***Math.round*** :làm tròn
***Math.floor*** :làm tròn xuống số nguyên gần nhất
***Math.ceil*** :làm tròn lên số nguyên gần nhất

###Random số 
***Math.random***: Random 1 số trong khoảng 0 --> 1

### Và các phương thức khác
```js
console.log(Math.pow(2,4))// Tính số mũ 2 mũ 4

console.log(Math.sqrt(16))// Căn bậc 2 của 16

console.log(Math.abs(-4))// GTTD của âm 4

// Math.max : Trả về lớn nhất trong một dãy số
console.log(Math.max(1,2,3,10,9,100))

// Math.min : Trả về nhỏ nhất trong một dãy số
console.log(Math.min(1,2,3,10,9,100))
```
 [Xem thêm](http://https://www.w3schools.com/js/js_math.asp)
