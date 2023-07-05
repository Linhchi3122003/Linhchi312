# JavaScript là một ngôn ngữ lập trình phía máy khách (client-side) được sử dụng chủ yếu để làm cho các trang web trở nên tương tác và động.

- Biến (Variables): Biến trong JavaScript được sử dụng để lưu trữ giá trị. Để khai báo một biến, bạn có thể sử dụng các từ khóa như `var`, `let` hoặc `const`

```
  var x = 5; // khai báo biến x với giá trị là 5
  let y = 10; // khai báo biến y với giá trị là 10
  const z = 15; // khai báo hằng số z với giá trị là 1
```
- Kiểu dữ liệu (Data Types): JavaScript hỗ trợ nhiều kiểu dữ liệu như số (number), chuỗi (string), mảng (array), đối tượng (object), boolean và null/undefined. Kiểu dữ liệu của biến có thể thay đổi trong quá trình thực thi. Ví dụ:
```
var number = 10; // kiểu dữ liệu số
var name = "John"; // kiểu dữ liệu chuỗi
var arr = [1, 2, 3]; // kiểu dữ liệu mảng
var person = { name: "John", age: 30 }; // kiểu dữ liệu đối tượng
var flag = true; // kiểu dữ liệu boolean
var empty = null; // kiểu dữ liệu null
var undef = undefined; // kiểu dữ liệu undefined
```
- Câu lệnh điều kiện (Conditional Statements): JavaScript cung cấp các câu lệnh điều kiện để thực hiện các hành động khác nhau dựa trên điều kiện. Câu lệnh `if`, `else if` và `else` thường được sử dụng. Ví dụ
```
var age = 18;

if (age < 18) {
    console.log("Bạn chưa đủ tuổi.");
} else if (age >= 18 && age < 21) {
    console.log("Bạn đủ tuổi để lái xe, nhưng chưa đủ tuổi để uống rượu.");
} else {
    console.log("Bạn đã đủ tuổi.");
}
```
- Vòng lặp (Loops): JavaScript cung cấp các vòng lặp để lặp lại một khối mã nhiều lần. Các vòng lặp thường được sử dụng bao gồm `for`, `while` và `do-while`. Ví dụ
```
for (var i = 0; i < 5; i++) {
    console.log(i); // in ra giá trị của i từ 0 đến 4
}

var j = 0;
while (j < 5) {
    console.log(j); // in ra giá trị của j từ 0 đến 4
    j++;
}
```
- Hàm (Functions): Hàm cho phép đóng gói một khối mã để thực hiện một tác vụ cụ thể. Bạn có thể định nghĩa hàm bằng từ khóa function. Ví dụ
```
function sayHello(name) {
    console.log("Xin chào, " + name + "!");
}

sayHello("John"); // Kết quả: "Xin chào, John!"
```
- Mảng (Arrays): Mảng là một cấu trúc dữ liệu trong JavaScript để lưu trữ nhiều giá trị trong một biến. Mỗi phần tử trong mảng có một chỉ số (index) duy nhất bắt đầu từ 0. Ví dụ:
```
var numbers = [1, 2, 3, 4, 5]; // một mảng các số
var names = ["John", "Jane", "Bob"]; // một mảng các chuỗi
var mixed = [1, "hello", true]; // một mảng gồm các kiểu dữ liệu khác nhau

console.log(numbers[0]); // truy cập vào phần tử đầu tiên của mảng (số 1)
console.log(names.length); // lấy độ dài của mảng (số phần tử trong mảng)
```
- Phương thức của mảng (Array Methods): JavaScript cung cấp nhiều phương thức để làm việc với mảng, ví dụ như `push()`, `pop()`, `shift()`, `unshift()`, `splice()`, `slice()`, `forEach()`, `map()`, và nhiều phương thức khác. Ví dụ
```
var fruits = ["apple", "banana", "orange"];

fruits.push("grape"); // thêm phần tử "grape" vào cuối mảng
fruits.pop(); // xóa phần tử cuối cùng của mảng
fruits.shift(); // xóa phần tử đầu tiên của mảng
fruits.unshift("watermelon"); // thêm phần tử "watermelon" vào đầu mảng

var citrus = fruits.slice(1, 3); // cắt mảng từ vị trí 1 đến 2 (không bao gồm 3)
fruits.splice(1, 2, "kiwi", "melon"); // xóa 2 phần tử từ vị trí 1 và thêm "kiwi" và "melon" vào vị trí đó

fruits.forEach(function(fruit) {
    console.log(fruit); // lặp qua mỗi phần tử trong mảng và in ra giá trị
});

var upperCaseFruits = fruits.map(function(fruit) {
    return fruit.toUpperCase(); // biến đổi mỗi phần tử trong mảng thành chữ hoa
});
```
- Đối tượng (Objects): Đối tượng là một cấu trúc dữ liệu phức tạp trong JavaScript, cho phép lưu trữ thông tin dưới dạng cặp khóa-giá trị. Đối tượng được định nghĩa bởi một tập hợp các thuộc tính (properties) và phương thức (methods). Ví dụ
```
var person = {
    name: "John",
    age: 30,
    greet: function() {
        console.log("Hello, my name is " + this.name + " and I'm " + this.age + " years old.");
    }
};

console.log(person.name); // truy cập vào thuộc tính "name" của đối tượng (giá trị là "John")
person.greet(); // gọi phương thức "greet" của đối tượng
```
- Sự kiện và xử lý sự kiện (Events and Event Handling): JavaScript cho phép bạn tương tác với người dùng thông qua các sự kiện như click chuột, submit form, di chuột qua một phần tử, và nhiều sự kiện khác. Bạn có thể gán các hàm xử lý sự kiện cho các phần tử HTML để thực thi mã JavaScript khi sự kiện xảy ra. Ví dụ
```
var button = document.getElementById("myButton");

button.addEventListener("click", function() {
    console.log("Button clicked!");
});
```
