# 🔥 FIRE-CHECK – ระบบแจ้งเตือนคุณภาพอากาศและขออนุญาตเผา

[![Made with Node.js](https://img.shields.io/badge/Backend-Node.js-green?logo=node.js)](https://nodejs.org)  
[![Machine Learning](https://img.shields.io/badge/ML-RandomForest-blue)](#)  
[![View Report](https://img.shields.io/badge/Report-PDF-orange)](https://drive.google.com/file/d/1XDfMwunoZ6GU5HttCTvx8zPCDHgMNzA5/view?usp=sharing)

**FIRE-CHECK** คือระบบต้นแบบที่ช่วยเกษตรกรและเจ้าหน้าที่ในการตรวจสอบคุณภาพอากาศ (PM2.5) และยื่นขออนุญาตเผาอย่างถูกต้องตามขั้นตอน โดยใช้ Machine Learning ในการคาดการณ์สภาพอากาศ พร้อมระบบ Email แจ้งเตือนและระบบจัดการผู้ใช้

---

## 📚 Table of Contents

- [🎯 วัตถุประสงค์ของระบบ](#-วัตถุประสงค์ของระบบ)
- [🛠 เทคโนโลยีที่ใช้](#-เทคโนโลยีที่ใช้)
- [🧠 ฟีเจอร์เด่น](#-ฟีเจอร์เด่น)
- [📁 โครงสร้างโปรเจกต์](#-โครงสร้างโปรเจกต์)
- [🚀 เริ่มต้นใช้งาน](#-เริ่มต้นใช้งาน)
- [📷 ตัวอย่างหน้าจอ](#-ตัวอย่างหน้าจอ)
- [📄 รายงานโปรเจกต์](#-รายงานโปรเจกต์)
- [👨‍💻 ผู้พัฒนา](#-ผู้พัฒนา)
- [📌 License](#-license)

---

## 🎯 วัตถุประสงค์ของระบบ

- ช่วยให้เกษตรกรสามารถตรวจสอบ PM2.5 ก่อนเผาเศษวัชพืช
- ให้เจ้าหน้าที่สามารถพิจารณาคำขอเผาได้ง่ายและโปร่งใส
- ลดปัญหาฝุ่นละอองในพื้นที่เกษตรกรรม
- ใช้เทคโนโลยี Machine Learning ในการคาดการณ์ PM2.5

---

## 🛠 เทคโนโลยีที่ใช้

| หมวดหมู่         | รายละเอียด                    |
|------------------|-------------------------------|
| Backend API      | Node.js + Express.js          |
| Machine Learning | Python (Random Forest)        |
| Database         | MongoDB                       |
| External API     | OpenWeather API               |
| Authentication   | JWT (Token-based Login)       |
| Email System     | Nodemailer                    |
| Tools            | Git, Postman, VS Code         |

---

## 🧠 ฟีเจอร์เด่น

- ✅ ตรวจสอบคุณภาพอากาศเรียลไทม์
- 📊 ระบบ ML คาดการณ์ค่าฝุ่น PM2.5
- 📩 Email Verification และแจ้งเตือนสถานะ
- 🔐 ระบบสิทธิ์ผู้ใช้งาน (Admin / User)
- 📄 ฟอร์มขออนุญาตเผาออนไลน์
- 📁 ประวัติการขออนุญาตย้อนหลัง

---

## 📁 โครงสร้างโปรเจกต์ (บางส่วน)

fire-check/ 
├── backend/ 
│   ├── controllers/ 
│   ├── models/ 
│   ├── routes/ 
│   ├── ml_model/ ← ML Script (Python) 
│   ├── config/ 
│   ├── server.js 
│   └── .env.example 
└── README.md

---

## 🚀 เริ่มต้นใช้งาน

### 1. Clone โปรเจกต์

```bash
git clone https://github.com/Wikorn1234/fire-check-pm25.git
cd fire-check-pm25/backend
```
### 2. ติดตั้ง Dependencies

npm install

### 3. สร้างไฟล์ .env

PORT=5000
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
EMAIL_USER=your_email
EMAIL_PASS=your_email_password

### 4. เริ่มรันระบบ

npm run dev

## 📷 ตัวอย่างหน้าจอ

(ใส่รูปหรือข้อมูลที่ต้องการแสดงตรงนี้)

## 📄 รายงานโปรเจกต์
📑 ดาวน์โหลดเอกสารรายงานฉบับเต็ม:
👉 [คลิกเพื่อดูไฟล์ PDF](https://drive.google.com/file/d/1XDfMwunoZ6GU5HttCTvx8zPCDHgMNzA5/view?usp=sharing)

## 👨‍💻 ผู้พัฒนา
วิกรม์ เหมเชื้อ (Wikorn Hemchuea)
- 📧 Email: wikorn134440@gmail.com
- 🔗 GitHub: [Wikorn1234](https://github.com/Wikorn1234)

## 📌 License
Distributed under the MIT License. See LICENSE for more information.
