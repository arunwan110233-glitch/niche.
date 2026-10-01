# NICHE — Micro-Talent Agency

ต้นแบบเว็บไซต์ภาษาไทยสำหรับ MBA พร้อมพอร์ตครีเอเตอร์ Talent CRM ฐานข้อมูลลูกค้า เครื่องคำนวณส่วนแบ่ง และ Business Blueprint

## เผยแพร่บน GitHub Pages
1. สร้าง repository ของคุณ แล้วแตก ZIP นี้และอัปโหลดไฟล์ทั้งหมดโดยคงโครงสร้างโฟลเดอร์ไว้บน branch `main` (รวม `.github/workflows/pages.yml`)
2. เปิด Settings > Pages > Build and deployment > Source แล้วเลือก GitHub Actions
3. เปิด Actions > Publish NICHE to GitHub Pages > Run workflow หากการรันครั้งแรกยังไม่สำเร็จก่อนตั้งค่า Pages
4. เมื่อสำเร็จ ลิงก์เว็บไซต์จะแสดงใน Settings > Pages และหน้า deployment

GitHub Free รองรับ Pages จาก repository แบบ Public; repository แบบ Private ต้องใช้แผนที่รองรับ ตรวจสอบสิทธิ์และการมองเห็นเว็บไซต์ก่อนเผยแพร่

## เปิดบนเครื่อง
รัน `python3 -m http.server 8000 --directory dist` แล้วเปิด http://localhost:8000

## ขอบเขต
ข้อมูลและบุคคลทั้งหมดเป็นตัวอย่าง ภาพประกอบสร้างด้วย AI ไม่ใช่ประวัติบุคคลจริง การเปลี่ยนแปลงข้อมูลอยู่ในหน่วยความจำและหายเมื่อรีเฟรช UTM ยังไม่เก็บคลิกหรือเชื่อมยอดขายจริง ไม่มีระบบบัญชีผู้ใช้หรือฐานข้อมูลฝั่งเซิร์ฟเวอร์

## ไฟล์
- dist/index.html: หน้าเว็บไซต์
- dist/style.css: รูปแบบและ responsive layout
- dist/app.js: การทำงานของต้นแบบ
- dist/images/: ภาพครีเอเตอร์
- .github/workflows/pages.yml: เผยแพร่เมื่อ push ไป main

อ้างอิง: https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages
