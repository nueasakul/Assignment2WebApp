# Drone Log Web (Assignment #2)

เว็บไซต์สำหรับดู config ของโดรน บันทึกอุณหภูมิ และดูประวัติ log

**Deployment:** `<https://nueasakul.github.io/Assignment2WebApp/>`

## การตั้งค่า

แก้ที่ต้นไฟล์ `script.js`

```js
const API_BASE = ...   // URL ของ API
const DRONE_ID = '67010999';
```

## วิธี run กรณี localhost

1. ติดตั้ง Node.js 18 ขึ้นไป
2. เปิดโฟลเดอร์ใน VS code แล้วสร้าง terminal โดยใช้ command prompt แล้วรัน `npm install`
3. สร้างไฟล์ `.env` ในโฟล์เดอร์เดียวกัน แล้วใส่ค่าจริง
   ```
   PORT=3000
   CONFIG_URL=<URL ของ Drone Config Server>
   LOG_URL=<URL ของ Drone Log Server>
   LOG_API_TOKEN=<Bearer token>
   ```
4. `npm start`
5. ใช้ส่วนเสริม **Live Server** กด Go Live ที่ไฟล์ index.html