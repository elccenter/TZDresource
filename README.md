# 📚 TZD · แผนที่ทรัพยากรการศึกษา

ระบบแดชบอร์ดแสดงแหล่งทรัพยากรการศึกษารายจังหวัด สำหรับ **Case Manager** โครงการ **Thailand Zero Dropout (TZD)**  
พัฒนาโดยความร่วมมือระหว่าง กสศ. และ ELC/Mahidol University

🔗 **[เปิดใช้งาน → yourname.github.io/tzd-resources](https://yourname.github.io/tzd-resources)**

---

## ✨ ฟีเจอร์หลัก

| ฟีเจอร์ | รายละเอียด |
|---|---|
| 🗺️ แผนที่ประเทศไทย | แสดงความหนาแน่นทรัพยากรรายจังหวัด (Choropleth) คลิกเลือกจังหวัดได้ |
| 📊 กราฟความก้าวหน้า | Coverage ring + Regional stacked bar chart แยก 6 ภูมิภาค |
| 📍 Province Dashboard | อันดับ, %, สัดส่วนตามประเภท เมื่อเลือกจังหวัด |
| 🔍 ค้นหา & กรอง | ค้นตามชื่อ, ประเภท, รูปแบบการศึกษา แบบ real-time |
| 📋 รายการทรัพยากร | การ์ดข้อมูล คลิกดูรายละเอียดได้ |
| 📤 Export ข้อมูล | Copy-to-clipboard แบบ TSV สำหรับ paste ลง Excel |
| 📱 Mobile-friendly | รองรับทั้ง Desktop และมือถือ |

---

## 📁 โครงสร้างไฟล์

```
tzd-resources/
│
├── index.html        ← แอปหลัก (self-contained, ไม่ต้อง server)
├── README.md         ← ไฟล์นี้
└── .nojekyll         ← บอก GitHub ไม่ต้องประมวลผล Jekyll
```

> ข้อมูลทรัพยากรทั้งหมดฝังอยู่ใน `index.html` ไม่ต้องการ database หรือ backend

---

## 🚀 วิธีเปิดใช้งาน (GitHub Pages)

1. Fork หรือ Upload ไฟล์ทั้งหมดไปยัง Repository ใหม่
2. ไปที่ **Settings → Pages**
3. ตั้ง Source เป็น **main branch**
4. รอ 1–2 นาที → เข้าใช้งานผ่าน URL ที่ได้รับ

---

## 🛠️ เทคโนโลยีที่ใช้

- **HTML / CSS / JavaScript** — ล้วนๆ ไม่มี framework
- **Leaflet.js** — แผนที่ interactive (CDN)
- **Thailand GeoJSON** — ขอบเขตจังหวัด 77 จังหวัด (embedded)
- **IBM Plex Sans Thai + Sarabun** — ฟอนต์ภาษาไทย (Google Fonts CDN)

---

## 📊 ข้อมูลในระบบ

- **476 แหล่งทรัพยากร** จาก **62 จังหวัด**
- แยกประเภท: วิชาชีพ (192) · วิชาการ (193) · วิชาชีวิต (88)
- แยกรูปแบบ: ในระบบ · นอกระบบ · ตามอัธยาศัย

---

## 👥 กลุ่มเป้าหมายผู้ใช้

- **Case Manager (CM)** — ค้นหาทรัพยากรเพื่อวาง Care Plan ให้เด็กรายบุคคล
- **ผู้ดูแลระบบ TZD** — ติดตามความครอบคลุมรายจังหวัดและภูมิภาค
- **ทีมส่วนกลาง กสศ.** — ภาพรวมระดับประเทศ

---

## 📝 หมายเหตุ

- ข้อมูลอ้างอิงจากฐานข้อมูล TZD ณ ช่วงเวลาที่รวบรวม
- หากต้องการอัปเดตข้อมูล ให้แทนที่ `const DATA = [...]` ใน `index.html`
- ระบบนี้ไม่เก็บข้อมูลผู้ใช้ ไม่มี cookies ไม่มี analytics

---

*พัฒนาสำหรับโครงการ Thailand Zero Dropout · กองทุนเพื่อความเสมอภาคทางการศึกษา (กสศ.)*
