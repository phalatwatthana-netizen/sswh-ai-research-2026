# SSWH AI Research 2026

เว็บแอประบบแบบประเมินความพึงพอใจ + ใบประกาศนียบัตร + แดชบอร์ดสรุปผล
สำหรับโครงการพัฒนางานประจำสู่งานวิจัยโดยใช้ปัญญาประดิษฐ์
เครือข่ายโรงพยาบาลศรีสังวรสุโขทัย จังหวัดสุโขทัย ประจำปี 2568

## ฟีเจอร์

- **แบบประเมิน** — ฟอร์มประเมินความพึงพอใจ ดึงตัวเลือกจาก Google Sheets และบันทึกผ่าน Google Apps Script
- **ใบประกาศ** — ค้นหารายชื่อแบบ autocomplete และบันทึกใบประกาศเป็น JPG / PDF
- **แดชบอร์ด** — สรุปผลด้วยกราฟ (Chart.js) พร้อมส่งออกรายงาน A4 เป็น JPG / PDF

## เทคโนโลยี

เป็น static site (ไฟล์เดียว `index.html`) ใช้ Tailwind CSS, Chart.js,
html2canvas และ jsPDF ผ่าน CDN — ไม่ต้อง build

## Deploy ผ่าน Netlify

1. เข้า [Netlify](https://app.netlify.com/) แล้วเลือก **Add new site → Import an existing project**
2. เชื่อมต่อกับ GitHub และเลือก repository นี้
3. ระบบจะอ่านค่าจาก `netlify.toml` ให้อัตโนมัติ:
   - **Build command:** ไม่ต้องใส่ (static site)
   - **Publish directory:** `.`
4. กด **Deploy** — Netlify จะ deploy ทุกครั้งที่ push ขึ้น GitHub

## ไฟล์ในโปรเจกต์

- `index.html` — เว็บแอปทั้งหมด
- `netlify.toml` — การตั้งค่า Netlify
