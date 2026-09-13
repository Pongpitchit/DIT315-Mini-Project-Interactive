# Solar Odyssey: Interactive Universe

## Slide 1 — แนวคิดโครงงาน

- โลกเสมือน: นิทรรศการระบบสุริยะที่เดินสำรวจได้
- เป้าหมาย: สแกน Earth และ Mars เพื่อปลดล็อก International Space Station (ISS)
- ผู้ใช้ไม่ได้เพียงชมฉาก แต่ต้องค้นหา เลือก อ่านข้อมูล และโต้ตอบกับวัตถุ

## Slide 2 — Environment และวัตถุ 3 มิติ

- Environment: spaceport, วงโคจร, asteroid belt และ sky texture แบบ 360°
- Primitive: ดวงอาทิตย์, ดาวเคราะห์ครบ 8 ดวง, ดวงจันทร์, วงแหวน Saturn และ asteroid
- 3D Model: `nasa-iss.glb` และ `satellite.gltf`
- ใช้ `position`, `rotation`, `scale` เพื่อสร้างระยะลึกและการจัดวาง

## Slide 3 — การควบคุมและรูปลักษณ์

- กล้องใช้ `look-controls` ให้มองรอบทิศ และ `wasd-controls` ให้เดินสำรวจ
- Cursor ใช้เล็งและคลิกวัตถุ class `clickable`
- ปรับ material ด้วย color, metalness, roughness และ emissive
- Sky ใช้ texture ที่อยู่ใน `images/stars-360.jpg`

## Slide 4 — Animation

- ดวงอาทิตย์และดาวเคราะห์หมุนรอบตัวเองอย่างต่อเนื่อง
- โลก, Mars, Jupiter และ Saturn เคลื่อนที่ตามวงโคจร
- ดวงจันทร์โคจรรอบโลก และ probe ลอยขึ้น-ลง
- เมื่อสแกนดาว จะมี animation ขยาย-ย่อเป็น feedback

## Slide 5 — Interaction และภารกิจ

1. คลิกโลกเพื่อสแกนข้อมูล
2. คลิกดาวอังคารเพื่อสแกนข้อมูล
3. คลิกดาวดวงอื่นเพื่ออ่านข้อมูล
4. เมื่อสแกนครบ 2 ดวง คลิก ISS เพื่อจบภารกิจ

## Slide 6 — สรุป

- ครบ Environment, วัตถุ Primitive + 3D Model, การเคลื่อนที่, animation และ interaction
- ไฟล์ทั้งหมดอยู่ในโฟลเดอร์โปรเจกต์ และเปิดผ่าน Live Server ได้
