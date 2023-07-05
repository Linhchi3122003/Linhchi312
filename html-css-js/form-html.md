 ## Thẻ trong HTML form:

1. `<form>`: Thẻ `<form>` được sử dụng để tạo một form trong HTML. Nó bao quanh các phần tử form khác và định nghĩa các thuộc tính và hành động của form. Ví dụ:

   ```html
   <form action="/process-form" method="POST">
     <!-- Các phần tử form nằm trong đây -->
   </form>
   ```

   - Thuộc tính `action`: Xác định URL hoặc đường dẫn đích xử lý form khi người dùng nhấn vào nút gửi.
   - Thuộc tính `method`: Xác định phương thức HTTP được sử dụng để gửi dữ liệu, ví dụ "GET" hoặc "POST".

2. `<input>`: Thẻ `<input>` được sử dụng để tạo các trường nhập dữ liệu trong form. Có nhiều giá trị cho thuộc tính `type` để xác định loại dữ liệu được nhập vào. Ví dụ:

   ```html
   <input type="text" name="username">
   ```

   - `type="text"`: Tạo một trường nhập văn bản.
   - `type="password"`: Tạo một trường nhập mật khẩu.
   - `type="email"`: Tạo một trường nhập địa chỉ email.
   - `type="checkbox"`: Tạo một ô kiểm (checkbox) cho lựa chọn nhiều giá trị.
   - `type="radio"`: Tạo một nút radio cho lựa chọn đơn giản.

3. `<label>`: Thẻ `<label>` được sử dụng để tạo nhãn cho các trường dữ liệu trong form. Nó liên kết với trường dữ liệu tương ứng bằng cách sử dụng thuộc tính `for` và `id`. Ví dụ:

   ```html
   <label for="username">Tên người dùng:</label>
   <input type="text" id="username" name="username">
   ```

4. `<textarea>`: Thẻ `<textarea>` được sử dụng để tạo trường nhập dữ liệu dạng văn bản nhiều dòng trong form. Ví dụ:

   ```html
   <textarea name="message" rows="4" cols="40"></textarea>
   ```

   - Thuộc tính `rows`: Xác định số hàng của trường dữ liệu.
   - Thuộc tính `cols`: Xác định số cột của trường dữ liệu.

5. `<select>` và `<option>`: Thẻ `<select>` được sử dụng để tạo một trường chọn (dropdown) trong form. Các tùy chọn được định nghĩa bên trong các thẻ `<option>`. Ví dụ:

   ```html
   <select name="country">
     <option

 value="vn">Việt Nam</option>
     <option value="us">Mỹ</option>
     <option value="jp">Nhật Bản</option>
   </select>
   ```

6. `<button>`: Thẻ `<button>` được sử dụng để tạo các nút trong form. Nó có thể được sử dụng cho các nút gửi form, nút đặt lại form hoặc các nút tùy chỉnh khác. Ví dụ:

   ```html
   <button type="submit">Gửi</button>
   ```
   - Thuộc tính `type`: Xác định loại nút, ví dụ "submit" hoặc "reset".