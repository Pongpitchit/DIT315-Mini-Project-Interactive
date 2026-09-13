# Solar Odyssey: Interactive Universe

โปรเจกต์ A-Frame แบบ Interactive Virtual World ฉบับปรับปรุง เป็นจักรวาลขนาดเล็กที่ผู้ใช้เดินสำรวจระบบสุริยะ อ่านข้อมูลดาวเคราะห์ และทำภารกิจปลดล็อกสถานีอวกาศนานาชาติ (ISS)

## วิธีเปิดใช้งาน

1. เปิดโฟลเดอร์นี้ด้วย VS Code
2. ใช้ส่วนขยาย **Live Server** เปิดไฟล์ `index.html` หรือเปิดผ่าน local web server
3. คลิก **Go Live** แล้วเปิด URL ที่แสดงในเบราว์เซอร์

> A-Frame, texture และ 3D model อยู่ในโฟลเดอร์โปรเจกต์ทั้งหมด จึงเปิดใช้งานแบบออฟไลน์ได้ผ่าน local web server

## วิธีเล่น

- ลากเมาส์/ลากนิ้วเพื่อมองรอบทิศทาง และใช้ `W A S D` เพื่อเดิน
- เล็ง cursor ไปที่ดาวเคราะห์แล้วคลิกเพื่อเปิดข้อมูลและเอฟเฟกต์เลือกวัตถุ
- ใช้ปุ่ม `HOME / EARTH / MARS / JUPITER / SATURN` สำหรับ fast travel หรือเดินสำรวจเอง
- สแกน **Earth** และ **Mars** ให้ครบ จากนั้นคลิก **ISS** เพื่อจบภารกิจ

## ตรวจตามข้อกำหนด

| ข้อกำหนด | การทำงานในโปรเจกต์ |
|---|---|
| Environment | Spaceport, วงโคจร, asteroid belt และ sky texture แบบ 360° |
| 3D objects ≥ 5 | ดวงอาทิตย์, ดาวเคราะห์ 8 ดวง, ดวงจันทร์, วงแหวน Saturn, asteroid, ISS และ probe |
| Primitive + 3D model | A-Frame primitives, `models/satellite.gltf` และ NASA ISS `.glb` |
| Position / Rotation / Scale | กำหนดให้วัตถุทุกกลุ่มใน `index.html` |
| Appearance | material, color, metalness, roughness, emissive และ texture ดาวจริง |
| สำรวจโลก | `look-controls`, `wasd-controls`, camera cursor |
| Animation ≥ 2 | ดวงอาทิตย์/ดาวเคราะห์หมุน, วงโคจร, ดวงจันทร์โคจร, Mars และ probe ลอย |
| Interaction ≥ 2 | ข้อมูลดาวเคราะห์, สแกน Earth, สแกน Mars, ปลดล็อกและคลิก ISS |

## โครงสร้างไฟล์

```text
.
├── index.html
├── aframe.min.js
├── README.md
├── Slide.md
├── images/stars-360.jpg
├── models/nasa-iss.glb
├── models/satellite.gltf
└── textures/
    ├── earth-atmos.jpg, moon.jpg, sun.jpg
    ├── jupiter.jpg, saturn.jpg
    └── saturn-ring.png
```

## ที่มาของ assets

- ภาพ texture ดาวและ sky: [Solar System Scope Textures](https://www.solarsystemscope.com/textures/) — CC BY 4.0
- โมเดล `nasa-iss.glb`: [NASA 3D Resources](https://science.nasa.gov/3d-resources/international-space-station-iss-a/) — NASA ระบุว่าสามารถดาวน์โหลดและใช้งานได้
- `satellite.gltf` เป็นโมเดล local ที่สร้างสำหรับโปรเจกต์นี้
