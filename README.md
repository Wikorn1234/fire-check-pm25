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
```bash
FIRE-CHECK/
├── config/
│   └── limits.json
├── models/
│   └── model_random_forest_ipn.joblib
├── node_modules/
├── public/
├── routes/
│   ├── admin.js
│   ├── auth.js
│   └── predict.js
├── uploads/
├── views/
│   ├── about.ejs
│   ├── admin_dashboard.ejs
│   ├── admin_invite.ejs
│   ├── admin_register.ejs
│   ├── burning.ejs
│   ├── contact.ejs
│   ├── detail_request.ejs
│   ├── history_request_admin.ejs
│   ├── history_request_officer.ejs
│   ├── history_request.ejs
│   ├── index.ejs
│   ├── login_process.ejs
│   ├── login.ejs
│   ├── logout.ejs
│   ├── officer_dashboard.ejs
│   ├── officer_details.ejs
│   ├── register_process.ejs
│   ├── register.ejs
│   ├── submit_request.ejs
│   ├── submit-contact.ejs
│   └── user_details.ejs
├── .gitignore
├── addAdminUser.js
├── database.js
├── emailVerifier.js
├── index.js
├── initializeConfig.js
├── package-lock.json
├── package.json
├── README.md
├── testEmailAPI.js
└── weather.js
```
---

## 🚀 เริ่มต้นใช้งาน

### 1. Clone โปรเจกต์

```bash
git clone https://github.com/Wikorn1234/fire-check-pm25.git
cd fire-check-pm25/backend
```
### 2. ติดตั้ง Dependencies
```bash
npm install
```
### 3. สร้างไฟล์ .env
```bash
PORT=5000
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
EMAIL_USER=your_email
EMAIL_PASS=your_email_password
```
### 4. เริ่มรันระบบ
```bash
npm run dev
```
## 📷 ตัวอย่างหน้าจอ
![Screenshot 2024-06-27 203319](https://github.com/user-attachments/assets/6b1a1992-8ede-4d6c-8d3d-79d9dfebe984)
![Screenshot 2024-06-27 203419](https://github.com/user-attachments/assets/8ea7f90f-c064-4e49-86a1-8db2a9948283)
![Screenshot 2024-06-27 203357](https://github.com/user-attachments/assets/c7bd4caa-66e8-4862-aaf3-31b2d84bc3c4)
![Screenshot 2024-06-28 080634](https://github.com/user-attachments/assets/a996d902-adb8-4e34-8135-2fc37861e1bb)
![Screenshot 2024-06-28 081102](https://github.com/user-attachments/assets/f0486327-8a37-4336-a4d0-3fbeedd626b7)
![Screenshot 2024-06-29 132902](https://github.com/user-attachments/assets/bdf72fb8-9fa7-4b8f-9914-91197327dba7)


## 📄 รายงานโปรเจกต์
📑 ดาวน์โหลดเอกสารรายงานฉบับเต็ม:
👉 [คลิกเพื่อดูไฟล์ PDF](20240715-ดอกดารารัตน์-BSCS66T2-15-620710130-620710682.pdf)

## 👨‍💻 ผู้พัฒนา
วิกรม์ เหมเชื้อ (Wikorn Hemchuea)
- 📧 Email: wikorn134440@gmail.com
- 🔗 GitHub: [Wikorn1234](https://github.com/Wikorn1234)

## 📌 License
Distributed under the MIT License. See LICENSE for more information.
