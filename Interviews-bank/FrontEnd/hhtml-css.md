## 📘 interview-bank/frontend/html-css.md

- <b>Author: `@Vinhdev04`</b><br><br>
  ![Interview Banner](../Images/banner-fe.jpg)

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

### ❓ Câu hỏi: "Box model trong CSS là gì?"

✅ Trả lời:
Box model là cấu trúc hình hộp của một phần tử HTML trong CSS, bao gồm các lớp từ trong ra ngoài: `content` → `padding` → `border` → `margin`.

📝 Điều quan trọng là mỗi phần tử đều bị ảnh hưởng bởi box model khi tính kích thước hoặc margin/padding.

🔥 Độ khó: ★☆☆☆☆  
🏷️ Tags: #css #box-model #layout

---

### ❓ Câu hỏi: "Sự khác biệt giữa absolute, relative, fixed và sticky là gì?"

✅ Trả lời:

- `relative`: định vị so với vị trí ban đầu
- `absolute`: định vị so với phần tử cha gần nhất có position (không thì so với viewport)
- `fixed`: định vị cố định theo viewport
- `sticky`: chuyển từ relative sang fixed khi scroll đến một ngưỡng nhất định

🔥 Độ khó: ★★☆☆☆  
🏷️ Tags: #css #position #layout

---

### ❓ Câu hỏi: "Specificity trong CSS là gì?"

✅ Trả lời:
Specificity là mức độ ưu tiên của một selector khi áp dụng style. Thứ tự ưu tiên:

1. Inline style
2. ID selector
3. Class, pseudo-class, attribute
4. Element tag

Ví dụ: `#id > .class > tag` → specificity: 100 > 10 > 1

🔥 Độ khó: ★★☆☆☆  
🏷️ Tags: #css #specificity #selector
