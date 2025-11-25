# ENGCE301
Software Design and Development (MintTea group 7)
# Members
1. นางสาว วชิรานีย์ ประเสริฐศรี 66543206052-3 [[GitHub]](https://github.com/wachipr)
2. นาย จิรภัทร จันทร์เทพ 66543206023-4 [[GitHub]](https://github.com/Tar8505)
3. นาย นฤชิต ไชยมงคล 66543206012-7 [[GitHub]](https://github.com/Fifachaimong)
4. นาย อานุภาพ เฑียรประยูร 66543206094-5 [[GitHub]](https://github.com/Muad2003)

# File
- [ENVIRONMENT.md](./ENVIRONMENT.md)
- [SE_INTRO_NOTES.md](./SE_INTRO_NOTES.md)

## DevTools Reflection (Week 1)

### 1) Browser รู้ได้อย่างไรว่าต้องรัน JavaScript ใน `<script>` เมื่อโหลดหน้าเว็บ?
**ตอบ**  
เมื่อ Browser โหลด HTML จะอ่านโครงสร้างเอกสารจากบนลงล่าง เมื่อเจอแท็ก `<script>` จะต้องหยุดการ parse ทุกอย่าง และให้รัน JavaScript ตามมาตรฐาน HTML Parsing Rules เมื่อทำงานในส่วนของ JavaScript เสร็จจึงจะกลับมา parser ต่อ 

---

### 2) ถ้าไม่มี DevTools การแก้ไขปัญหา (debug) เวลาเว็บมีปัญหาจะยากขึ้นอย่างไร?
**ตอบ**  
1. ทำให้นักพัฒนาไม่รู้ว่าปัญหาหรือบั๊กที่เจออยู่ เกิดจากอะไร ทำให้เสียเวลามากขึ้น  
2. หากเกิดปัญหาโหลดช้า หรือ Performance ตกต้องค้นหาด้วยตัวเองว่า ส่วนไหนของโปรแกรมที่โหลดช้า  
3. ไม่สามารถตรวจ Layout และ CSS ได้ ทำให้แก้ปัญหา Layout หรือ Style ผิดตำแหน่งได้ยาก  

---

### 3) แต่ละคนคิดว่า Panel ไหนใน DevTools จะได้ใช้บ่อยที่สุดในเทอมนี้ (Elements / Console / Network / อื่น ๆ)? เพราะอะไร?
**ตอบ**  
- (วชิรานีย์)  **Console Network** เพราะ ไว้สำหรับดู error ของ backend และดูload ของระบบlocalที่เราเขียนว่ามีload อะไรขึ้นไปบ้างและเกิดerrorจรงจุดไหนบ้าง ก่อนจะขึ้นระบบจริง
- (จิรภัทร)  **Elements** เพราะใช้จัด layout และ debug UI
- (นฤชิต)  **Console** เพราะน่าจะได้ใช้ตรวจสอบค่าบ่อยถ้าเกิดมีอะไรผิดพลาด
- (อานุภาพ) **Console** เพราะ ดู error JS และเช็คตัวแปร
