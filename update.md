ทำครบตาม mission.md แล้ว — เปิด index.html ผ่าน Live Server / local web server ได้ และมีไฟล์ครบตามที่ส่งงานกำหนด

ข้อกำหนด	สถานะ	ในโปรเจกต์
Environment (Ground / Sky / 360°)
ครบ
a-sky จาก images/stars-360.jpg + พื้น spaceport (a-cylinder / a-ring)
วัตถุ 3D ≥ 5 + Primitive และ 3D Model
ครบ
Primitive: ดวงอาทิตย์, ดาวเคราะห์, ดวงจันทร์, วงแหวน, asteroid, พื้นที่ยาน — Model: models/nasa-iss.glb, models/satellite.gltf
Position, Rotation, Scale
ครบ
วางดาวด้วย position/rotation; ISS และ probe ใช้ scale ด้วย
Appearance (Color / Material / Texture)
ครบ
สี + metalness/roughness/emissive + texture ใน textures/
มองรอบและเดินสำรวจ
ครบ
look-controls + wasd-controls + cursor
Animation ≥ 2
ครบ (เกิน)
หมุนตัว, โคจร, ดวงจันทร์โคจร, Mars ลอย, probe ลอย, cursor scale
Interaction ≥ 2
ครบ (เกิน)
คลิกดาวดูข้อมูล, สแกน Earth/Mars, คลิก ISS จบภารกิจ, ปุ่ม fast travel
index.html + images/ + models/ + textures/
ครบ
มีครบทั้งสามโฟลเดอร์และไฟล์หลัก
Comment จุดสำคัญใน HTML
ครบ
comment บล็อก scene และสคริปต์ interaction
ไฟล์ที่ HTML โหลดจริงมีอยู่ครบ: stars-360.jpg, texture ดวงอาทิตย์/โลก/ดวงจันทร์/พฤหัส/เสาร์/วงแหวน, nasa-iss.glb, satellite.gltf

ไฟล์ที่ไม่ถูกใช้งาน (`images/space-panorama.svg` และ `textures/moon-surface.jpg`) ถูกตรวจสอบ reference แล้วลบออกเพื่อให้โฟลเดอร์สะอาด

หมายเหตุตอนเปิด: ต้องใช้ web server (ไม่เปิดไฟล์ตรงจาก Explorer) และต้องมีเน็ตครั้งแรกเพื่อโหลด A-Frame จาก CDN ตามที่ README ระบุแล้ว
