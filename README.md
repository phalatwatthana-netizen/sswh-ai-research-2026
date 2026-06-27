# SSWH AI Research 2026

เว็บไซต์ static เริ่มต้น เชื่อมต่อ GitHub กับ Netlify

## Deploy ผ่าน Netlify

1. เข้า [Netlify](https://app.netlify.com/) แล้วเลือก **Add new site → Import an existing project**
2. เชื่อมต่อกับ GitHub และเลือก repository นี้
3. ตั้งค่า build ตามนี้ (ระบบจะอ่านจาก `netlify.toml` ให้อัตโนมัติ):
   - **Build command:** ไม่ต้องใส่ (static site)
   - **Publish directory:** `.`
4. กด **Deploy** — Netlify จะ deploy ทุกครั้งที่ push ขึ้น GitHub

## ไฟล์ในโปรเจกต์

- `index.html` — หน้าเว็บหลัก
- `netlify.toml` — การตั้งค่า Netlify
