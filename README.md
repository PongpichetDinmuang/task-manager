# Task Manager

A lightweight, privacy-first task manager that runs entirely in your browser — no installation, no account, no internet required.

แอปจัดการแผนงานแบบเบาๆ ที่รันในเบราว์เซอร์ล้วนๆ ไม่ต้องติดตั้ง ไม่ต้องสมัครสมาชิก ไม่ต้องต่ออินเทอร์เน็ต

---

## 🚀 Getting Started / วิธีใช้งาน

### Desktop
1. Download `task_manager.html`
2. Double-click to open in your browser
3. Start adding tasks

### Mobile (iPhone / Android)
Open the link below in **Safari** or **Chrome**:

👉 **[https://your-username.github.io/your-repo/task_manager.html](https://your-username.github.io/your-repo/task_manager.html)**

> Replace the URL with your own GitHub Pages link.

---

## ✨ Features / ฟีเจอร์

### 📋 Task Management / จัดการงาน
- Add, edit, and delete tasks / เพิ่ม แก้ไข ลบงานได้
- Add a description to each task / ใส่รายละเอียดงานได้
- Set a deadline with date and time / ตั้ง deadline วันและเวลา

### ✅ Subtasks / รายการย่อย
- Break tasks into subtasks / แตกงานเป็นรายการย่อยได้
- Check off subtasks to track progress / ติ๊กเพื่อบอกว่าทำเสร็จแล้ว
- Progress percentage auto-calculated / คำนวณ % ความคืบหน้าอัตโนมัติ

### 🔴 Auto Urgency / ความเร่งด่วนอัตโนมัติ
Urgency is calculated automatically from the deadline — no manual setting needed.

ระบบคำนวณความเร่งด่วนจาก deadline อัตโนมัติ ไม่ต้องตั้งเอง

| Time Remaining / เวลาที่เหลือ | Level / ระดับ | Color / สี |
|---|---|---|
| < 48 hours / ชั่วโมง | Critical / วิกฤต | 🔴 Red |
| < 72 hours / ชั่วโมง | High / สูง | 🟠 Orange |
| < 7 days / วัน | Medium / ปานกลาง | 🟡 Yellow |
| 7+ days / วันขึ้นไป | Low / ต่ำ | 🟢 Green |
| Progress 100% | Done / เสร็จแล้ว | ✅ |

### 📅 Calendar View / มุมมองปฏิทิน
- Monthly calendar highlighting deadline dates / ปฏิทินรายเดือน ไฮไลต์วัน deadline
- Tap a task in the calendar to view details / กดงานในปฏิทินเพื่อดูรายละเอียด

### 📊 Overview Dashboard / ภาพรวม
- Summary stats: total, done, critical tasks / สรุปสถิติงานทั้งหมด เสร็จแล้ว วิกฤต
- Overall progress bar across all tasks / progress bar รวมทุกงาน
- Tasks sorted by deadline / เรียงงานตาม deadline อัตโนมัติ

### 💾 Save & Load Data / บันทึกและโหลดข้อมูล
- **Desktop Chrome**: Save directly to any folder on your computer / บันทึกลง folder ที่เลือกได้เลย
- **Mobile / Other browsers**: Download `tasks_data.json` and load it back next time / ดาวน์โหลด JSON แล้วโหลดกลับมาได้

---

## 🔒 Privacy / ความเป็นส่วนตัว

- All data stays on **your device only** / ข้อมูลทั้งหมดอยู่ในเครื่องของคุณเท่านั้น
- No data is sent to any server / ไม่มีการส่งข้อมูลออกอินเทอร์เน็ต
- No cookies, no tracking, no ads / ไม่มี cookies ไม่มีการติดตาม ไม่มีโฆษณา
- No browser storage (localStorage) used / ไม่ใช้ localStorage ของเบราว์เซอร์

Your data lives in `tasks_data.json` — a file you own and control.

ข้อมูลทั้งหมดอยู่ใน `tasks_data.json` ซึ่งเป็นไฟล์ที่คุณดูแลเองทั้งหมด

---

## 📁 File Structure / โครงสร้างไฟล์

```
📁 your-folder/
├── task_manager.html    ← Open this / เปิดไฟล์นี้
└── tasks_data.json      ← Your data / ข้อมูลของคุณ (สร้างเมื่อกด Save)
```

---

## 🌐 Browser Support / เบราว์เซอร์ที่รองรับ

| Browser | Desktop | Mobile |
|---|---|---|
| Chrome | ✅ Full (direct save to folder) | ✅ |
| Safari | ✅ | ✅ |
| Edge | ✅ Full (direct save to folder) | ✅ |
| Firefox | ✅ (download/upload) | ✅ |

---

## 🛠️ Built With / เทคโนโลยีที่ใช้

- Pure HTML, CSS, JavaScript — no frameworks, no dependencies
- [Tabler Icons](https://tabler.io/icons) for icons
- File System Access API (Chrome/Edge desktop)

---

*Made with ❤️ — simple tools for a focused life.*
