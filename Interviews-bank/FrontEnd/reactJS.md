## 📘 interview-bank/frontend/react.md

- <b>Author: `@Vinhdev04`</b><br><br>
  ![Interview Banner](../Images/banner-react.webp)

> 🧠 "Chuẩn bị phỏng vấn bài bản – Tự tin chiến thắng vòng Technical"

---

## 💼 Giới thiệu Series

Series này tổng hợp những **câu hỏi thường gặp trong phỏng vấn IT**, kèm theo **phân tích và lời giải thích chi tiết**, giúp bạn:

- Ôn lại kiến thức nền tảng quan trọng
- Hiểu cách diễn đạt câu trả lời logic, ngắn gọn
- Tránh lỗi tâm lý/phát biểu sai khi phỏng vấn
- Làm quen với tình huống phỏng vấn thực tế

---

🔥 Độ khó: ★★☆☆☆ <br>
🏷️ Tags: #database #nosql #design

---

### ❓ Câu hỏi: "React Hook useEffect dùng để làm gì?"

✅ Trả lời:
`useEffect` dùng để xử lý các side-effect (fetch API, thao tác DOM, subscriptions...) sau khi component render. Có thể kiểm soát thời điểm chạy bằng cách truyền dependencies array.

Ví dụ:

```js
useEffect(() => {
  document.title = `Bạn có ${count} tin nhắn`;
}, [count]);
```

🔥 Độ khó: ★★☆☆☆  
🏷️ Tags: #react #hook #useEffect #side-effect

---

### ❓ Câu hỏi: "Virtual DOM là gì và hoạt động như thế nào trong React?"

✅ Trả lời:
Virtual DOM là một bản sao nhẹ của DOM thật. Khi state thay đổi, React sẽ:

1. Tạo virtual DOM mới
2. So sánh với virtual DOM cũ (diffing)
3. Tính toán sự khác biệt (reconciliation)
4. Cập nhật DOM thật tối thiểu

🔥 Độ khó: ★★☆☆☆  
🏷️ Tags: #react #virtual-dom #performance

---

### ❓ Câu hỏi: "State và Props khác nhau như thế nào?"

✅ Trả lời:

- `State`: dữ liệu nội bộ, có thể thay đổi bằng `setState` hoặc hook `useState`
- `Props`: dữ liệu truyền từ component cha xuống, không thể thay đổi trong component con

🔥 Độ khó: ★☆☆☆☆  
🏷️ Tags: #react #state #props #component
