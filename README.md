# ร้านไอดี One Piece 🗡️

เว็บแอพจัดการสต็อกไอดีวันพีช ซิงค์ real-time ผ่าน Firebase

---

## วิธี Deploy (ทำครั้งเดียวพอ!)

### ขั้นตอนที่ 1 — สร้าง Firebase

1. ไปที่ https://console.firebase.google.com
2. กด **"Add project"** → ตั้งชื่อ เช่น `onepiece-shop`
3. ปิด Google Analytics (ไม่จำเป็น) → **Create project**
4. ใน sidebar ซ้าย → **Build** → **Realtime Database**
5. กด **"Create database"** → เลือก **test mode** → **Enable**
6. ไปที่ **Project Settings** (ไอคอนฟัน ⚙️ ข้าง Project Overview)
7. เลื่อนลงมา **"Your apps"** → กด **`</>`** (Web icon)
8. ลงทะเบียน app (ชื่ออะไรก็ได้) → คัดลอก **firebaseConfig** เก็บไว้

### ขั้นตอนที่ 2 — Deploy บน Vercel

1. ไปที่ https://vercel.com → สมัครด้วย GitHub (ฟรี)
2. กด **"Add New Project"**
3. เลือก **"Deploy from existing file"** หรือ อัพโหลดโฟลเดอร์นี้
   - ถ้าไม่มี GitHub: ใช้ Vercel CLI → `npx vercel` ใน folder นี้
4. รอ deploy → จะได้ URL เช่น `https://onepiece-shop.vercel.app`

### ขั้นตอนที่ 3 — เชื่อมต่อ Firebase

1. เปิดเว็บที่ได้จาก Vercel
2. ระบบจะถามหา Firebase config
3. วาง JSON ที่คัดลอกจาก Firebase → กด **เชื่อมต่อ**
4. เสร็จ! ใช้ได้เลย ทั้งตัวเองและแฟน

---

## วิธีให้แฟนใช้

- ส่ง Vercel URL ให้แฟน (เช่น https://onepiece-shop.vercel.app)
- แฟนเปิด URL → ใส่ Firebase config เดียวกัน → เชื่อมต่อ
- ข้อมูลซิงค์ real-time ทั้ง 2 เครื่อง ✅

---

## ฟีเจอร์

- ✅ ดูสต็อกไอดีที่เหลือ แยก Android / iOS
- ✅ กด "ขายแล้ว" → lock ทันที ป้องกันขายซ้ำ
- ✅ เพิ่มไอดีใหม่ได้ตลอดเวลา
- ✅ ดูประวัติการขายทั้งหมด
- ✅ ซิงค์ real-time ผ่าน Firebase
