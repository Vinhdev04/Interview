## 📘 interview-bank/frontend/javascript.md

- <b>Author: `@Vinhdev04`</b><br><br>
  ![Interview Banner](../Images/banner-js.png)

> 🧠 "Hiểu sâu JavaScript – Vượt qua mọi vòng phỏng vấn"

---

## 💼 Giới thiệu Series

Series này giúp bạn:

- Làm chủ nền tảng JavaScript từ cơ bản đến nâng cao
- Tránh các lỗi thường gặp và hiểu kỹ cơ chế hoạt động bên trong JS
- Có thể tự tin giải thích các khái niệm với nhà tuyển dụng

---

### ❓ Câu hỏi: "So sánh var, let và const trong JavaScript"

✅ Trả lời:

- `var`: khai báo biến toàn cục hoặc function scope, có thể bị hoisting
- `let`: block scope, không hoisting như var
- `const`: giống let nhưng không gán lại được

| Từ khóa | Scope    | Hoisting | Gán lại | Khởi tạo lại |
| ------- | -------- | -------- | ------- | ------------ |
| var     | function | Có       | Có      | Có           |
| let     | block    | Không    | Có      | Không        |
| const   | block    | Không    | Không   | Không        |

🔥 Độ khó: ★☆☆☆☆  
🏷️ Tags: #javascript #scope #variable

---

### ❓ Câu hỏi: "JavaScript closure là gì?"

✅ Trả lời:
Closure là function ghi nhớ được biến bên ngoài khi nó được tạo ra, ngay cả khi function đó được gọi ngoài phạm vi ban đầu.

Ví dụ:

```js
function outer() {
  let counter = 0;
  return function inner() {
    counter++;
    return counter;
  };
}
const count = outer();
console.log(count()); // 1
console.log(count()); // 2
```

📝 Closure giúp tạo private variable và các pattern như memoization, module pattern.  
🔥 Độ khó: ★★★☆☆  
🏷️ Tags: #closure #javascript #function

---

### ❓ Câu hỏi: "Sự khác nhau giữa == và === trong JS là gì?"

✅ Trả lời:

- `==`: so sánh bằng giá trị, có ép kiểu
- `===`: so sánh bằng cả giá trị và kiểu dữ liệu (strict equality)

```js
"5" == 5; // true
"5" === 5; // false
```

🔥 Độ khó: ★☆☆☆☆  
🏷️ Tags: #equality #type-coercion #javascript

---

### ❓ `Câu hỏi 01: .  DOM trong HTML được hiểu như thế nào? Nêu một số DOM Event bạn đã biết?`

✅ Trả lời:<br>

- `DOM` là Document-Object-Modal -> là Mô hình Các Đối Tượng Tài Liệu<br>
  ![](../Images/dom-la-gi.gif)<br>
- <b>`Câu trúc DOM`:</b>
  - Node: Document node - Element node - Text node
  - Một node có thể có một hoặc nhiều con, nhưng cũng có thể không có con nào.
  - Những node có cùng node cha được gọi là các node anh em `siblings`.
  - Trong các node anh em, node đầu tiên được gọi là con cả `firstChild` và node cuối cùng là con út `lastChild`. <br><br>
    ![](../Images/Example-of-DOM-Node-Tree.png)<br>
- <b>`Các loại DOM trong Javascript`:</b>
  - `DOM Document:` lưu trữ toàn bộ các thành phần trong documents của website
  - `DOM Element:` truy xuất tới thẻ HTML nào đó thông qua các thuộc tính như tên class, id, name của thẻ HTML.
  - `DOM HTML:` thay đổi giá trị nội dung và giá trị thuộc tính của các thẻ HTML.
  - `DOM CSS:` thay đổi các định dạng CSS của thẻ HTML.
  - `DOM Event:` gán các sự kiện như onclick(), onload() vào các thẻ HTML.
  - `DOM Listener:` lắng nghe các sự kiện tác động lên thẻ HTML.
  - `DOM Navigation:` dùng để quản lý, thao tác với các thẻ HTML, thể hiện mối quan hệ cha – con của các thẻ HTML
  - `DOM Node,NodeList:` thao tác với HTML thông qua đối tượng (Object).
- <b>`Thuộc tính quan hệ:`</b>
  - `parentNode`: node cha
  - `childNodes`: Các node con
  - `firstChild`: node con đầu tiên
  - `lastChild`: node con cuối cùng
  - `nextSibling`: node anh em liền kề sau
  - `previousSibling`: node anh em liền kề trước
- `DOM (Document Object Model)` là một mô hình dạng cây (tree structure) đại diện cho toàn bộ nội dung của tài liệu HTML. Khi trình duyệt tải một trang web, nó tạo ra một cây DOM, trong đó:

- Mỗi thẻ HTML là một node (nút).

- Nội dung bên trong là text node.

- Có thể truy cập, thay đổi, thêm hoặc xóa các phần tử HTML bằng JavaScript thông qua DOM.

👉 Hiểu đơn giản: DOM chính là cách JavaScript "thấy" và "tương tác" với trang web.
