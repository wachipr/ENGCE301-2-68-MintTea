Software Requirements Specification (SRS)\
ระบบสั่งอาหารในมหาวิทยาลัย / CampusEats

ENGCE301: การออกแบบและพัฒนาซอฟต์แวร์\
Software Design and Development

Term Project - Group 7

ชื่อ-นามสกุล รหัสนักศึกษา Role นางสาววชิรานีย์ ประเสริฐศรี 66543206052
-3 ผู้ใช้ทั่วไป\
นายจิรภัทร จันทร์เทพ 66543206023 -4 บุคลากร\
นายนฤชิต ไชยมงคล 66543206012 -7 นักศึกษา\
นายอานุภาพ เฑียรประยูร 66543206094 -5 ผู้ดูแลระบบ

Version: 1.0\
Date: 27 พฤศจิกายน 2568 มหาวิทยาลัยเทคโนโลยีราชมงคลล้านนา\
Rajamangala University of Technology Lanna

Document Control\
Version History\
Version Date Author Description of Change\
1.0 27/11/2026 วชิรานีย์ , จิรภัทร,\
นฤชิต, อานุภาพ Initial draft

Document Approvals\
Role Name Signature & Date\
Product Owner วชิรานีย์\
Team Lead วชิรานีย์\
Instructor อ.ธนิต

Table of Contents\
เนื้อหา\
Document Control ................................
................................ ................................
................................ ...... 2 Version History
................................ ................................
................................ ................................
......... 2 Document Approvals ................................
................................ ................................
............................ 2 Table of Contents
................................ ................................
................................ ................................
....... 3 1. Introduction ................................
................................ ................................
................................ ............. 5 1.1 Purpose
................................ ................................
................................ ................................
.............. 5 1.2 Scope ................................
................................ ................................
................................ .................. 5 1.3 Definitions,
Acronyms, and Abbreviations ................................
................................ ................ 6 1.4 References
................................ ................................
................................ ................................
......... 6 1.5 Overview ................................
................................ ................................
................................ ............ 7 2. Overall Description
................................ ................................
................................ ................................ 8 2.1
Product Perspective ................................
................................ ................................
........................ 8 2.2 Product Functions
................................ ................................
................................ ......................... 10 2.3 User
Characteristics ................................
................................ ................................
.......................11 2.4 Constraints
................................ ................................
................................ ................................
.......11 2.5 Assumptions and Dependencies
................................ ................................
.............................. 12 3. Specific Requirements
................................ ................................
................................ ........................ 13 3.1
Functional Requirements ................................
................................ ................................
............13 3.1.1 User Authentication Module
................................ ................................
.............................. 13 3.2 Non -Functional Requirements
................................ ................................
................................ ...20

3.2.1 Performance Requirements ................................
................................ ................................ 20
3.2.2 Security Requirements ................................
................................ ................................
.........20 3.2.3 Usability Requirements
................................ ................................
................................ ........20 3.2.4 Reliability
Requirements ................................
................................ ................................
......20 3.2.5 Portability Requirements ................................
................................ ................................
.....20 4. Appendices ................................
................................ ................................
................................ ............22 4.1 Use Case Diagrams
................................ ................................
................................ ........................ 22 4.2
Wireframes / Mockups ................................
................................ ................................
.................26 4.3 Data Dictionary ................................
................................ ................................
............................... 26 4.4 User Interview Notes Summary
................................ ................................
................................ .31 5. Glossary
................................ ................................
................................ ................................
...................34 การใช้งาน Template นี้
................................ ................................
................................ .............................. 39

1.  Introduction\
    1.1 Purpose\
    เอกสารฉบับนี้ระบุความต้องการ ( Requirements)
    ของระบบระบบสั่งอาหารในมหาวิทยาลัย มีวัตถุประสงค์เพื่อ\
    • ใช้เป็นแนวทางในการออกแบบ ( Design) และพัฒนา (Development)
    ระบบสั่งอาหารออนไลน์ , จองโต๊ะ , รีวิวร้านอาหาร ภายในมหาวิทยาลัย\
    • ใช้เป็นเกณฑ์ในการทดสอบ ( Testing) และตรวจสอบความสมบูรณ์ของระบบ
    สั่งอาหารออนไลน์ , จอง โต๊ะ, รีวิวร้านอาหาร ภายในมหาวิทยาลัย\
    • ใช้เป็นสัญญาระหว่างทีมพัฒนากับผู้มีส่วนได้ส่วนเสีย (
    Stakeholders)\
    1.2 Scope\
    ระบบสั่งอาหารในมหาวิทยาลัย เป็น มือถือแอป ที่มีวัตถุประสงค์เพื่อ
    ให้นักศึกษาสามารถสั่ง อาหาร , จองโต๊ะ
    และรีวิวร้านอาหารภายในมหาวิทยาลัย\
    ขอบเขตของระบบครอบคลุม:\
    • ร ะบ บ ลงท ะเบ ีย น และเข ้ า ส ู ่ร ะบ บ ร อ งร ับ น ั ก ศ ึก ษ า
    และร ้ า น ค ้ า พ ร ้ อ ม ก า ร ย ืน ย ั น ต ั ว ต น เบ ื ้ อ งต ้
    น\
    • จ ั ด ก า ร โ ป ร ไ ฟ ล์ผู ้ ใ ช ้ แก ้ ไ ขข ้ อ ม ู ลส่วน ต ั ว
    เช ่น ช ื่อ เบ อ ร ์ โ ท ร ห ร ื อ ข ้ อ ม ู ลร ้ า น ค ้ า\
    • แสด งร า ย ก า ร ร ้ า น อ า ห า ร และเม น ู ผู ้ ใ ช ้ สามาร ถ ด
    ู เม น ู ร า ย ละเอีย ด ร า ค า และสถ า น ะอ า ห า ร\
    • ร ะบ บ ส ั่ งอ า ห า ร อ อ น ไ ลน ์ ช า ร ะเงิน และส่งค า ส ั่ งซ
    ื ้ อ ต ร งถ ึงร ้ า น ค ้ า ต ิด ต า ม สถ า น ะค า ส ั่ งซ ื ้ อ\
    • แสด งสถ า น ะ เช ่น ร อ ร ับ อ อ เด อ ร ์ ก า ล ั งท า เสร ็ จ แล
    ้ ว พ ร ้ อ ม ร ับ\
    • ร ะบ บ จ อ งโ ต ๊ ะใ น ร ้ า น อ า ห า ร เลือก ว ั น เวลา จ า น ว
    น ท ี่น ั่ ง และร ับ ก า ร ย ืน ย ั น จ า ก ร ้ า น ค ้ า\
    • ร ี ว ิว และค ะแน น ร ้ า น อ า ห า ร ผู ้ ใ ช ้ ใ ห ้ ด า ว และค
    อ ม เม น ต ์เก ี่ย ว ก ับ ร ้ า น อ า ห า ร\
    • ร ะบ บ แจ ้ งเต ือ น แจ ้ งเต ือ น สถ า น ะอ อ เด อ ร ์ โ ต ๊ ะจ อ
    ง ห ร ื อ โ ป ร โ ม ช ั่ น\
    • แ ด ช บ อ ร ์ ด ร ้ า น ค ้ า ร ้ า น ค ้ า ส า ม า ร ถ จ ัด ก า ร
    เม น ู เ พ ิ่ ม ห ร ื อ ลบ ร า ย ก า ร อ า ห า ร ต อ บ ร ั บ ห ร ื อ
    ย ก เลิ ก ออ เด อ ร ์ และด ู ร ี ว ิว ร า ย ก า ร อ า ห า ร

• ร ะบ บ ผู ้ ด ู แล ( Admin Panel) จ ั ด ก า ร ร ้ า น ค ้ า ผู ้ ใ ช ้
เม น ู และต ร ว จ สอบ ร ี ว ิว ไ ม ่เห ม า ะสม

ขอบเขตที่ไม่รวมในระบบ (Out of Scope):\
• ไ ม ่ร ว ม ร ะบ บ บ ร ิ ห า ร ว ั ต ถ ุด ิบ ภา ย ใ น ร ้ า น\
• ไ ม ่ร ว ม ร ะบ บ POS • ไ ม ่ร ว ม ร ะบ บ ก า ร ค ืน เงิน ต ้ อ งร ับ
เร ื่ อ งผ่าน ร ้ า น ค ้ า ห ร ื อ ผู ้ ด ู แล\
• ไ ม ่ร อ งร ั บ ร ะบ บ แ ผน ท ี่ แบ บ เ ร ี ย ล ไ ท ม ์ ( GPS) ไ ม ่ ม
ีก า ร ต ิ ด ต า ม ต า แห น ่ งผู ้ ส่ง ห ร ื อ ร ้ า น ค ้ า แบ บ แ อ ป
เด ลิ เวอ ร ี

1.3 Definitions, Acronyms, and Abbreviations\
Term Definition\
FR Functional Requirement\
NFR Non-Functional Requirement\
UI User Interface\
API Application Programming Interface\
SRS Software Requirements Specification\
Admin ผู้ดูแลระบบ\
1.4 References\
− IEEE Standard 830 -1998 - IEEE Recommended Practice for Software
Requirements Specifications\
• Brainstorming Session Minutes - บันทึกการประชุม Brainstorm (27 พ.ย.
2026)

1.5 Overview\
เอกสารนี้ประกอบด้วย 3 ส่วนหลัก:\
• Section 1 (Introduction) - แนะนำภาพรวมของเอกสารและโปรเจกต์\
• Section 2 (Overall Description) - อธิบายภาพรวมของระบบ\
• Section 3 (Specific Requirements) - ระบุความต้องการโดยละเอียด

2.  Overall Description\
    2.1 Product Perspective\
    ระบบ CampusEats -- ระบบสั่งอาหารในมหาวิทยาลัย เป็นระบบแบบ Web
    Application ทำงานบน Web Browser รองรับทั้งคอมพิวเตอร์และอุปกรณ์พกพา\
    ระบบมีการเชื่อมต่อกับ:\
    • API -- ใช้สำหรับการยืนยันตัวตนผ่าน Account ของนักศึกษา/บุคลากร
    RMUTL\
    • Custom Authentication via University Database -
    ระบบจะเชื่อมต่อกับฐานข้อมูลหรือบริการยืนยันตัวตนของมหาวิทยาลัย\
    • Database System -- เก็บข้อมูลผู้ใช้ ร้านค้า เมนูอาหาร
    และคำสั่งซื้อ เช่น SQL / Progress\
    

2.2 Product Functions\
ฟังก์ชันหลักของระบบ (สรุปย่อจาก Functional Requirements):\
1. User Registration - ผู้ใช้สามารถลงทะเบียนเข้าใช้ระบบด้วยรหัสนักศึกษา
รหัสผ่าน อีเมล และข้อมูลส่วนตัว\
2. User Login - ผู้ใช้เข้าสู่ระบบด้วย Student ID และ Password\
Update User Profile - ผู้ใช้สามารถแก้ไขข้อมูลส่วนตัว เช่น เบอร์โทร อีเมล
รูปโปรไฟล์ และข้อมูลติดต่อ\
3. Browse Restaurants & Menu -
ผู้ใช้สามารถดูรายการร้านอาหารและเมนูพร้อมรายละเอียด\
4. Place Food Order - ผู้ใช้ทำการสั่งอาหารในแอป\
5. Track Order Status - ผู้ใช้ติดตามสถานะคำสั่งซื้อ\
6. Place Food Order - ระบบตรวจสอบการชำระเงิน\
7. Table Reservation - ผู้ใช้จองโต๊ะกับร้าน\
8. Submit Review - ผู้ใช้ให้คะแนนและรีวิวร้านอาหารที่เคยสั่ง\
9. Restaurant Login - ร้านค้าเข้าสู่ระบบด้วย Restaurant ID ,Password\
10. Restaurant Menu Management - ร้านค้าจัดการเมนู เช่น เพิ่ม ลบ
หรือแก้ไขเมนู\
11. Restaurant Registration - Admin
จะสมัครบัญชีสำหรับการจัดการร้านค้าให้\
12. Admin Dashboard - Admin ดูภาพรวมของสถิตการสั่งอาหาร ,สถิติการจองโต๊ะ
และรีวิวของร้านอาหาร

2.3 User Characteristics\
กลุ่มผู้ใช้หลักของระบบ:\
User Type 1: นักศึกษาและบุคลากร มทร.ล้านนา\
• ลักษณะ: อายุ 18 --40 ปี มีพื้นฐานการใช้งานสมาร์ทโฟนและอินเทอร์เน็ต\
• ความเชี่ยวชาญด้านเทคโนโลยี: ระดับทั่วไปถึงระดับกลาง\
• วัตถุประสงค์การใช้งาน: ค้นหาเมนู สั่งอาหาร ชำระเงิน
และติดตามสถานะคำสั่งซื้อ\
User Type 2: ร้านค้าในโรงอาหาร\
• ลักษณะ: ผู้ประกอบการร้านอาหารในมหาวิทยาลัย อายุ 25 --55 ปี •
ความเชี่ยวชาญด้านเทคโนโลยี: ระดับพื้นฐาน --กลาง (ใช้งานผ่าน smart phone/
tablet / PC )\
• วัตถุประสงค์การใช้งาน:รับคำสั่งซื้อ จัดการเมนู อัปเดตสถานะอาหาร\
User Type 3: ผู้ดูแลระบบ\
• ลักษณะ: เจ้าหน้าที่ IT หรือผู้ที่รับผิดชอบด้านระบบ25 --60 ปี •
ความเชี่ยวชาญด้านเทคโนโลยี: ระดับสูง\
• วัตถุประสงค์การใช้งาน: ดูแลระบบรวมถึงข้อมูลร้านค้า รายงาน
และการกำหนดสิทธิ

2.4 Constraints\
ข้อจำกัดในการพัฒนาระบบ:\
งบประมาณ: "ไม่มีงบประมาณ ( Academic project)"\
เวลา: ต้องเสร็จภายในภาคการศึกษานี้ (สัปดาห์ที่ 16)\
เทคโนโลยี: ใช้ React, Node.js, SQLite/MongoDB\
มีเวลาทำงาน 4-6 ชม./สัปดาห์\
ต้องปฏิบัติตามกฎระเบียบด้านข้อมูลส่วนบุคคล ( PDPA)\
ต้องรองรับจำนวนผู้ใช้พร้อมกันระดับหลักร้อยภายในมหาวิทยาลัย

ทีมพัฒนา: มีสมาชิก 4 คน มีเวลาทำงาน 4 -6 ชม./สัปดาห์\
2.5 Assumptions and Dependencies\
สมมติฐาน (Assumptions):\
• ผู้ใช้มี Internet Connection ที่เสถียร\
• ผู้ใช้มี อุปกรณ์ที่รองรับ Web Browser เช่น Notebook / Smartphone\
• ร้านค้าที่เข้าร่วมโครงการสามารถใช้งานระบบผ่านอินเทอร์เน็ต
และมีอุปกรณ์สำหรับรับคำสั่งซื้อ\
• ระบบยืนยันตัวตนของมหาวิทยาลัย ( RMUTL Account API)
และฐานข้อมูลมหาวิทยาลัยพร้อมให้บริการตลอด

Dependencies ( สิ่งที่ระบบพึ่งพา):\
Custom Authentication via University Database s -
ใช้สำหรับตรวจสอบตัวตนผู้ใช้ โดยเชื่อมต่อกับบัญชีของนักศึกษาและบุคลากร\
React.js -- ใช้สร้าง Frontend UI เช่น หน้าสั่งอาหารและแดชบอร์ดร้านค้า\
Web Server สำหรับ Deploy เช่น Render, หรือของมหาวิทยาลัย)

3.  Specific Requirements\
    3.1 Functional Requirements\
    3.1.1 User Authentication Module\
    FR-001: User Registration\
    ID FR-001 Description ผู้ใช้สามารถลงทะเบียนเข้าใช้ระบบด้วย รหัส
    นักศึกษา รหัสผ่าน อีเมล และข้อมูลส่วนตัว\
    Input Student ID (format: xxxxxxxxxx -x), Password (min 8 chars),
    Email (xxxxx@xxxxx.xxx ), ชื่อ-นามสกุล\
    Process ตรวจสอบ Student ID ซ้ำ, ตรวจสอบ password strength, Hash
    password, บันทึก ข้อมูล Output สร้างบัญชีผู้ใช้ และส่งอีเมลยืนยัน\
    Precondition -\
    Priority Must Have\
    FR-002: User Login\
    ID FR-002 Description ผู้ใช้เข้าสู่ระบบด้วย Student ID และ Password\
    Input Student ID (format: xxxxxxxxxx -x), Password\
    Process ตรวจสอบข้อมูล , เปรียบเทียบ Hash password, ออก JWT Token\
    Output เข้าสู่ Dashboard พร้อม Token\
    Precondition ต้องลงทะเบียนแล้ว\
    Priority Must Have

FR-003: Update User Profile\
ID FR-003 Description ผู้ใช้สามารถแก้ไขข้อมูลส่วนตัว เช่น เบอร์โทร อีเมล
รูปโปรไฟล์ และข้อมูลติดต่อ\
Input Student Id, เบอร์โทรศัพท์ใหม่ , อีเมลใหม่ , รูป โปรไฟล์ ,
ข้อมูลส่วนบุคคลที่ต้องการแก้ไข\
Process ตรวจสอบความถูกต้องของข้อมูล , ตรวจสอบ Email ซ้ำ,
บันทึกข้อมูลอัปเดตลงฐานข้อมูล\
Output ระบบแสดงข้อความ "อัปเดตข้อมูลสำเร็จ"\
Precondition ผู้ใช้ต้องเข้าสู่ระบบ\
Priority Should Have\
3.1.2 Restaurants & Menu\
FR-004: Browse Restaurants & Menu\
ID FR-004 Description ผู้ใช้สามารถดูรายการร้านอาหารและเมนูพร้อม
รายละเอียด\
Input Restaurant ID\
Process ดึงข้อมูลร้าน และเมนูจากฐานข้อมูล\
Output แสดงเมนู ราคา รูปภาพ สถานะ\
Precondition ร้านค้าต้องมีเมนู active\
Priority Must Have

3.1.3 Food Order\
FR-005: Place Food Order\
ID FR-005 Description ผู้ใช้ทำการสั่งอาหารในแอป\
Input Menu Items List, รายการเมนู , จำนวน , วิธี ชำระเงิน\
Process ตรวจสอบเมนู , คำนวณราคา , บันทึกคำสั่งซื้อ\
Output หมายเลขคำสั่งซื้อ และสถานะเริ่มต้น\
Precondition ผู้ใช้ต้องเข้าสู่ระบบ\
Priority Must Have\
FR-006: Track Order Status\
ID FR-006 Description ผู้ใช้ติดตามสถานะคำสั่งซื้อแบบเรียลไทม์\
Input Order ID\
Process ตรวจสอบสถานะจากฐานข้อมูล\
Output สถานะคำสั่งซื้อ\
Precondition ต้องมีคำสั่งซื้อ\
Priority Must Have

3.1.4 Payment\
FR-007: Place Food Order\
ID FR-007 Description ระบบตรวจสอบการชำระเงิน\
Input Payment ID\
Process ตรวจสอบผ่าน API Payment Gateway\
Output แสดงผลการชำระเงิน\
Precondition คำสั่งซื้ออยู่ในสถานะรอชำระเงิน\
Priority Must Have\
3.1.5 Table\
FR-008: Table Reservation\
ID FR-008 Description ผู้ใช้จองโต๊ะกับร้าน\
Input Student ID, วันที่, เวลา, จำนวนคน , ร้านที่ ต้องการ\
Process ตรวจสอบโต๊ะว่าง , บันทึกคำขอจอง\
Output สถานะการจอง\
Precondition ผู้ใช้ต้องเข้าสู่ระบบ\
Priority Must Have

3.1.6 Review\
FR-009: Submit Review\
ID FR-009 Description ผู้ใช้ให้คะแนนและรีวิวร้านอาหารที่เคยสั่ง\
Input Restaurant ID, คะแนน , ข้อความ\
Process ตรวจสอบสิทธิ์ (เคยสั่งร้านนี้หรือไม่) , บันทึกรีวิว\
Output รีวิวถูกแสดงบนหน้าร้าน\
Precondition ต้องมีประวัติการสั่งอาหารร้านนั้น\
Priority Must Have\
3.1.7 Restaurant Management\
FR-010: Restaurant Login ID FR-010 Description ร้านค้าเข้าสู่ระบบด้วย
Restaurant ID\
,Password\
Input Restaurant ID ,Password\
Process ตรวจสอบข้อมูล , เปรียบเทียบ Hash password, ออก JWT Token\
Output เข้าสู่ Dashboard การจัดการเมนู\
Precondition ต้องลงทะเบียนแล้ว\
Priority Must Have

FR-011: Restaurant Menu Management\
ID FR-011 Description ร้านค้าจัดการเมนู เช่น เพิ่ม ลบ หรือแก้ไขเมนู\
Input Menu Id, ชื่อเมนู , ราคา, รูปภาพ , สถานะ\
Process บันทึกหรืออัปเดตเมนูในระบบ\
Output เมนูถูกปรับปรุงและแสดงผล\
Precondition ร้านค้าต้องเข้าสู่ระบบด้วยสิทธิ์ร้าน\
Priority Must Have\
1.1.8 Admin Management\
FR-012: Restaurant Registration\
ID FR-012 Description Admin จะสมัครบัญชีสำหรับการจัดการร้านค้าให้\
Input Restaurant ID ,Password\
Process ตรวจสอบ password strength, Hash password, บันทึกข้อมูล\
Output สร้างบัญชีสำหรับร้านค้า\
Precondition - Priority Must Have

FR-013: Admin Dashboard\
ID FR-013 Description Admin ดูภาพรวมของสถิตการสั่งอาหาร ,สถิติ
การจองโต๊ะ และรีวิวของร้านอาหาร\
Input Restaurant ID ,Review Id , Table Reservation ID\
Process ดึง log Database จากร้านค้านั้นมาสรุปสถิติทั้ง การสั่งอาหาร
จองโต๊ะ และการรีวิว\
Output Dashboard สถิติ Precondition ตรวจสอบสิทธิ์ Admin\
Priority Must Have

3.2 Non -Functional Requirements\
3.2.1 Performance Requirements\
ID Requirement Metric/Target\
NFR-001 Page Load Time หน้าเว็บต้องโหลดเสร็จภายใน 2 วินาที (วัดด้วย
Lighthouse)\
NFR-002 API Response Time API Response Time ต้องไม่เกิน 500 ms (95th
percentile)\
NFR-003 Concurrent Users ระบบต้องรองรับผู้ใช้พร้อมกัน 100 คน\
3.2.2 Security Requirements\
ID Requirement Implementation\
NFR-004 Password Security ใช้ bcrypt ในการ Hash (salt rounds ≥ 10)\
NFR-005 Session Management Session Token (JWT) ต้องมีอายุไม่เกิน 24 ชม.\
NFR-006 Data Encryption ต้องใช้ HTTPS สำหรับการสื่อสารทั้งหมด\
3.2.3 Usability Requirements\
• NFR-007: ผู้ใช้ต้องสามารถสั่งอาหาร (ฟีเจอร์หลัก) ได้ภายใน ≤ 3 คลิก •
NFR-008: UI ต้องรองรับ ภาษาไทย / อังกฤษ\
• NFR-009: ระบบต้องแสดง Error Message ที่เข้าใจง่ายพร้อม
คำแนะนำวิธีแก้ไข\
3.2.4 Reliability Requirements\
− NFR-010: ระบบต้องมี uptime 99% (downtime ไม่เกิน 3.65 วัน/ปี)\
• NFR-011: ทำ Backup อัตโนมัติทุก 24 ชั่วโมง\
• NFR-012: ระบบต้องสามารถ Recovery ภายใน 5 นาที
เมื่อเกิดปัญหาระดับทั่วไป

3.2.5 Portability Requirements\
• NFR-013: เว็บรองรับเบราว์เซอร์ Chrome, Firefox, Safari, Edge (latest
version)\
• NFR-014: รองรับความละเอียดทั้ง Desktop (1920×1080) , Tablet (768×1024)
, Mobile (375×667)\
• NFR-015: UI ต้องรองรับ Dark Mode / Light Mode\
3.2.7 Compliance Requirements\
− NFR-016: ก า ร เก ็บ ข ้ อ ม ู ลส่วน บ ุค ค ลต ้ อ งสอด ค ล ้ อ งต า ม
PDPA − NFR-017: เก ็บ Log ก า ร ใ ช ้ งา น ขอ งผู ้ ด ู แลร ะบ บ อ ย ่า
งน ้ อ ย 90 ว ั น − NFR-018: ข ้ อ ม ู ลส าค ั ญต ้ อ งไ ม ่ถ ูก แส ด
งใน log เช ่น password, token, payment info

4.  Appendices\
    4.1 Use Case Diagrams

คำอธิบาย Use Case CampusEats student/personnel/Product\
Use Case Title : Client Register Use Case ID : 1 Primary Actor : New
Students / Personnel\
Stakeholder Actor : Custom Authentication via University Database,
Identity\
Main Flow : ผู้ใช้้งาน 2กลุ่ม นักศึกษา และบุคลากร กดRegister
ระบบจะแสดงหน้าฟอร์ม Register ผู้ใช้กรอกข้อมูล แล้วผู้ใช้กดส่ง
ระบบตรวจสอบความถูกต้อง และบันทึกข้อมูลผู้ใช้ลงฐานข้อมูล

Use Case Title : Booking table Use Case ID : 2 Primary Actor : New
Students / Personnel, Register Students / Personnel\
Stakeholder Actor : Custom Authentication via University Database,
Identity\
Main Flow : ผู้ใช้เข้าสู่ระบบ เลือกเมนู " Booking Table"
ระบบแสดงรายการจองโต๊ะและช่วงเวลาที่ โต๊ะว่าง และสามารถเลือกโต๊ะ
จองโต๊ะและเวลาที่ต้องการ

Use Case Title : Make Order Use Case ID : 3

Primary Actor : Register Students / Personnel\
Stakeholder Actor : Custom Authentication via University Database,
Identity\
Main Flow : กดเมนู "Make Order" ระบบจะแสดงรายการอาหารจากร้านอาหาร
ผู้ใช้สามารถเลือกอาหาร เมื่อเลือกระบบจะเพิ่มรายการอาหาร
และจะแสดงรายการอาหารในตะกร้า

Use Case Title : Checkout Use Case ID : 4 Primary Actor : - Stakeholder
Actor : Custom Authentication via University Database, Identity ,
Payment\
Main Flow : ผู้ใช้เลือก "Checkout"
ระบบจะแสดงสรุปรายการอาหารและราคาทั้งหมด เลือกวิธีการชำระเงิน
ผู้ใช้ยืนยันการชำระเงิน ระบบทำรายการชำระเงินผ่านระบบ Payment\
บันทึกคำสั่งซื้อ และแสดงข้อความยืนยันการสั่งซื้อสำเร็จ

Use Case Title : View Menu Use Case ID : 5 Primary Actor : Register
Students / Personnel , Product\
Stakeholder Actor : Custom Authentication via University Database,
Identity\
Main Flow : กดเลือกเมนู "View Menu"
ระบบจะแสดงรายการอาหารทั้งหมดให้ผู้ใช้ดู

Use Case Title : Add/edit/delete product Use Case ID : 6 Primary Actor :
Product\
Stakeholder Actor : Custom Authentication via University Database,
Identity\
Main Flow : ร้านอาหารจะแสดงรายการอาหารของร้าน และสามารถเลือกเพิ่ม แก้ไข
หรือ ลบรายการอาหารได้

คำอธิบาย Use Case CampusEats Admin\
Use Case Title : Restaurant Register Use Case ID : 1 Primary Actor : New
Product\
Stakeholder Actor : Custom Authentication via University Database,
Identity\
Main Flow : การลงทะเบียนร้านอาหาร จะต้องให้ adminเป็นผู้ลงทะเบียน
adminจะสร้างบัญชีร้านอาหารให้แค่ ชื่อร้าน restaurant ID , password\
เพื่อให้ร้านไปเพิ่มรายละเอียดบัญชีหลังจาก admin สร้างบัญชีเสร็จ

Use Case Title : Admin Dashboard Use Case ID : 2 Primary Actor : Admin\
Stakeholder Actor : Custom Authentication via University Database,
Identity\
Main Flow : ระบบจะตรวจสอบสิทธิ์แอดมิน แสดงหน้า Dashboard พร้อมสรุปสถิติ
ของรายการทั้งหมด

Use Case Title : Manage Users Use Case ID : 3 Primary Actor : Admin\
Stakeholder Actor : Custom Authentication via University Database,
Identity\
Main Flow : Admin กดดูเมนู "Manage Users" ระบบจะแสดงรายชื่อผู้ใช้งาน และ
Adminสามารถ แก้ไขปรับเปลี่ยน หรือลบ บัญชีได้ ถ้าหากมีความจำเป็น

Use Case Title : Manage Menu Use Case ID : 4 Primary Actor : Admin\
Stakeholder Actor : Custom Authentication via University Database,
Identity\
Main Flow : Admin กดดูเมนู "Manage Menu" ระบบแสดงรายการเมนูอาหารทั้งหมด
Admin

สามารถ เพิ่ม แก้ไข หรือลบเมนู ถ้าหากมีความจำเป็น

Use Case Title : View Report Use Case ID : 5 Primary Actor : Admin\
Stakeholder Actor : Custom Authentication via University Database,
Identity\
Main Flow : Admin กดดูเมนู "View Report" ระบบดึงข้อมูลรายงาน เช่น
ยอดขายและจำนวนออเดอร์ของแต่ละร้าน หรือทั้งหมดในระบบ สามารถ
ดึงข้อมูลรายวัน, เดือน, และปีได้ ระบบจะแสดงรายงานในรูปแบบตาราง

4.2 Wireframes / Mockups

4.3 Data Dictionary\
ตารางอธิบายโครงสร้างข้อมูลสำคัญ:

Entity/Ta ble Attribute Data Type Description\
User user_id INT Primary Key, Auto- increment\
User student_id VARCHAR(12) รหัสนักศึกษา (format: xxxxxxxxxx -x),
Unique, Not Null User email VARCHAR(255) อีเมลผู้ใช้, Unique, Not Null
User password VARCHAR(255) รหัสผ่านที่ถูก Hash User first_name
VARCHAR(100) ชื่อผู้ใช้\
User last_name VARCHAR(100) นามสกุลผู้ใช้\
User phone_nu mber VARCHAR(20) เบอร์โทรศัพท์\
User profile_ima ge VARCHAR(255) URL รูปโปรไฟล์\
User created_at DATETIME วันที่สร้างบัญชี\
User updated_a t DATETIME วันที่แก้ไขล่าสุด\
Restaurant restaurant\_ id INT Primary Key, Auto- increment\
Restaurant name VARCHAR(255) ชื่อร้านอาหาร\
Restaurant email VARCHAR(255) อีเมลร้าน,

Unique\
Restaurant password VARCHAR(255) รหัสผ่านร้าน (Hash)\
Restaurant phone_nu mber VARCHAR(20) เบอร์โทรร้าน\
Restaurant address VARCHAR(255) ที่อยู่ร้าน\
Restaurant created_at DATETIME วันที่สร้างบัญชีร้า น Restaurant
updated_a t DATETIME วันที่แก้ไขล่าสุด\
Menu menu_id INT Primary Key, Auto- increment\
Menu restaurant\_ id INT Foreign Key Restaurant.rest aurant_id\
Menu name VARCHAR(255) ชื่อเมนู\
Menu price DECIMAL(10,2) ราคาต่อหน่วย\
Menu image_url VARCHAR(255) รูปภาพเมนู\
Menu status ENUM('active','inactive') สถานะเมนู\
Menu created_at DATETIME วันที่สร้างเมนู\
Menu updated_a t DATETIME วันที่แก้ไขล่าสุด\
Order order_id INT Primary Key, Auto- increment\
Order user_id INT Foreign Key User.user_id\
Order order_date DATETIME วันที่สั่งอาหาร

Order total_price DECIMAL(10,2) ราคารวมทั้งหมด\
Order status ENUM('pending','confirmed','preparing','deliver
ing','completed','cancelled') สถานะคำสั่งซื้อ\
Order payment_s tatus ENUM('pending','paid','failed') สถานะการชำระเ งิน
Order created_at DATETIME วันที่สร้างคำสั่งซื้ อ Order updated_a t
DATETIME วันที่แก้ไขล่าสุด\
OrderItem order_item *id INT Primary Key, Auto- increment\
OrderItem order_id INT Foreign Key\
Order.order_id\
OrderItem menu_id INT Foreign Key\
Menu.menu_id\
OrderItem quantity INT จำนวนรายการ\
OrderItem price DECIMAL(10,2) ราคาต่อรายการ\
Payment payment_i d INT Primary Key, Auto- increment\
Payment order_id INT Foreign Key\
Order.order_id\
Payment payment* method VARCHAR(50) วิธีชำระเงิน\
Payment amount DECIMAL(10,2) จำนวนเงิน\
Payment status ENUM('pending','completed','failed') สถานะการชำระเ งิน
Payment payment\_ DATETIME วันที่ชำระเงิน

date TableRese rvation reservation *id INT Primary Key, Auto- increment\
TableRese rvation user_id INT Foreign Key\
User.user_id\
TableRese rvation restaurant* id INT Foreign Key\
Restaurant.rest aurant_id\
TableRese rvation reservation \_date DATE วันที่จอง\
TableRese rvation reservation *time TIME เวลาในการจอง\
TableRese rvation num_peop le INT จำนวนคน\
TableRese rvation status ENUM('pending','confirmed','cancelled')
สถานะการจอง\
Review review_id INT Primary Key, Auto- increment\
Review user_id INT Foreign Key\
User.user_id\
Review restaurant* id INT Foreign Key\
Restaurant.rest aurant_id\
Review rating TINYINT คะแนน 1 -5 Review comment TEXT ข้อความรีวิว\
Review created_at DATETIME วันที่สร้างรีวิว\
Review updated_a DATETIME วันที่แก้ไขรีวิว

t

4.4 User Interview Notes Summary\
คนที่ 1 ผู้ใช้งานทั่วไป\
Pain Point : ผู้ใช้บริการร้านอาหารในมหาลัย โดยทั่วไปมีทั้งคนที่ มาติดต่อ
ราชการ หรือบุคคลภายนอก\
เมื่อต้องการใช้บริการร้านอาหารในมหาลัย\
มักจะประสบปัญหากับการใช้บริการโรงอาหารไม่มี พื้นที่นั่งเพียงพอ
เนื่องจากผู้ใช้บริการมีทั้ง นักศึกษา บุคลากร
ที่เข้าใช้บริการพร้อมกันเป็นจำนวนมาก\
Requirements :\
1. การเข้าสู่ระบบ ใช้งานสั่งอาหาร\
2. ระบบการสั่งอาหาร และ จองโต๊ะ\
3. ประวัติการจองโต๊ะ และ การสั่งอาหาร\
คนที่ 2 นักศึกษา\
Pain Point : นักศึกษาส่วนมากอยากได้ช่องทาง การชำระเงินที่มีความสะดว
กสบายมากขึ้น และ ต้องการแสดงความคิดเห็นที่มีต่อร้าน
อาหารที่เคยไปใช้บริการ\
Requirements :\
1.ระบบการชำระเงิน\
2.ช่องทางแสดงความคิดเห็นต่อ ร้านอาหาร

คนที่ 3 บุคลากร\
Pain Points : บุคลากรส่วนใหญ่ต้องการให้ทั้งนักศึกษา และ
บุคคลภายนอกที่มาใช้บริการร้านอาหารในมหาลัย โดยไม่ต้องรอนานหรือสามารถสั่ง
อาหารล่วงหน้า\
อีกทั้งยังติดตามคำสั่งซื้อได้ เพื่อความพึงพอใจของ
ผู้ที่มาใช้บริการร้านอาหาร\
Requirements :\
1.ระบบการสั่งซื้ออาหาร\
2.ระบบติดตามการสั่งซื้อ\
คนที่ 4 ร้านอาหาร\
Pain Points : พบปัญหาเมื่อมีผู้ใช้บริการจำนวนมาก
จึงส่งผลให้บางรายการอาหารที่ถู กมองข้าม หรือรายการที่เพิ่ มเข้ามาใหม่
จะถูกแนะนำในเว็ปไซต์สั่งอาหารในมหาลัย\
อีกทั้งเมื่อมีการสั่งรายการอาหารเข้ามา ทำให้ไม่ทันต่อจำนวนผู้สั่ง
ส่งผลให้มีการต่อคิวเป็นจำนวนมาก เกิดความล่าช้าและส่งผล
ต่อจำนวนโต๊ะที่นั่ง\
Requirements :\
1.ระบบแจ้งเตือนการสั่งอาหาร\
2.ระบบการตอบรับ หรือการยกเลิกคำสั่งซื้อ ของร้านอาหาร
(กรณีที่ร้านอาหารมีความจำเป็นต้องกด "ยกเลิก")

5.  Glossary\
    Term Definition\
    Admin ผู้ดูแลระบบของระบบ CampusEats\
    API Application Programming Interface --
    ชุดคำสั่งใช้เชื่อมต่อระบบต่าง ๆ\
    Authentication กระบวนการพิสูจน์ตัวตนของผู้ใช้ เช่น Login Dashboard
    หน้าจอสรุปข้อมูลสำหรับผู้ใช้หรือร้านค้า\
    Email Verification กระบวนการส่งอีเมลเพื่อยืนยันตัวตนหลังสมัคร
    สมาชิก\
    FR Functional Requirement -- ความต้องการเชิง ฟังก์ชัน\
    Hash กระบวนการแปลงข้อมูล (เช่น รหัสผ่าน) ให้เป็น
    รูปแบบที่ไม่สามารถย้อนกลับได้\
    JWT JSON Web Token -- Token ที่ใช้สำหรับยืนยัน สิทธิ์ผู้ใช้ (
    Session Token)\
    Menu Item รายการอาหารที่ร้านค้าเพิ่มในระบบ\
    NFR Non-Functional Requirement -- ความ ต้องการที่ไม่ใช่ฟังก์ชัน เช่น
    ความปลอดภัย ความเร็ว\
    Order Status สถานะของคำสั่งซื้อ (รอรับ , กำลังทำ , เสร็จแล้ว ฯลฯ)
    Payment Gateway บริการกลางสำหรับตรวจสอบและประมวลผลการ ชำระเงิน\
    PDPA กฎหมายคุ้มครองข้อมูลส่วนบุคคลของไทย\
    Reservation การจองโต๊ะในร้านอาหาร\
    Session สถานะการเข้าใช้งานของผู้ใช้ เช่น ขณะล็อกอิน\
    Stakeholder บุคคลที่เกี่ยวข้องหรือมีผลกระทบต่อระบบ

Term Definition\
Student ID รหัสนักศึกษาที่ใช้เป็นตัวตนหลักในการ ลงทะเบียน\
Token ข้อมูลที่ใช้แทนการเข้าสู่ระบบเพื่อเข้าถึง API UI User Interface --
ส่วนที่ผู้ใช้โต้ตอบกับระบบ เช่น ปุ่ม หน้าจอ ฟอร์ม\
User Authentication โมดูลการลงทะเบียนและเข้าสู่ระบบของผู้ใช้\
Validation การตรวจสอบความถูกต้องของข้อมูลที่ป้อน เช่น Email Format หรือ
Password Strength\
Term Definition\
Admin ผู้ดูแลระบบของระบบ CampusEats\
API Application Programming Interface -- ชุดคำสั่งใช้เชื่อมต่อระบบต่าง
ๆ\
Authentication กระบวนการพิสูจน์ตัวตนของผู้ใช้ เช่น Login Dashboard
หน้าจอสรุปข้อมูลสำหรับผู้ใช้หรือร้านค้า\
Email Verification กระบวนการส่งอีเมลเพื่อยืนยันตัวตนหลังสมัคร สมาชิก\
FR Functional Requirement -- ความต้องการเชิง ฟังก์ชัน\
Hash กระบวนการแปลงข้อมูล (เช่น รหัสผ่าน) ให้เป็น
รูปแบบที่ไม่สามารถย้อนกลับได้\
JWT JSON Web Token -- Token ที่ใช้สำหรับยืนยัน สิทธิ์ผู้ใช้ ( Session
Token)\
Menu Item รายการอาหารที่ร้านค้าเพิ่มในระบบ\
NFR Non-Functional Requirement -- ความ ต้องการที่ไม่ใช่ฟังก์ชัน เช่น
ความปลอดภัย

ความเร็ว

Term Definition\
Order Status สถานะของคำสั่งซื้อ (รอรับ, กำลังทำ , เสร็จแล้ว ฯลฯ) Payment
Gateway บริการกลางสำหรับตรวจสอบและประมวลผลการ ชำระเงิน\
PDPA กฎหมายคุ้มครองข้อมูลส่วนบุคคลของไทย\
Reservation การจองโต๊ะในร้านอาหาร\
Session สถานะการเข้าใช้งานของผู้ใช้ เช่น ขณะล็อกอิน\
Stakeholder บุคคลที่เกี่ยวข้องหรือมีผลกระทบต่อระบบ\
Student ID รหัสนักศึกษาที่ใช้เป็นตัวตนหลักในการ ลงทะเบียน\
Token ข้อมูลที่ใช้แทนการเข้าสู่ระบบเพื่อเข้าถึง API UI User Interface --
ส่วนที่ผู้ใช้โต้ตอบกับระบบ เช่น ปุ่ม หน้าจอ ฟอร์ม\
User Authentication โมดูลการลงทะเบียนและเข้าสู่ระบบของผู้ใช้\
Validation การตรวจสอบความถูกต้องของข้อมูลที่ป้อน เช่น\
Email Format หรือ Password Strength\
Term Definition\
Admin ผู้ดูแลระบบของระบบ CampusEats\
API Application Programming Interface -- ชุดคำสั่งใช้เชื่อมต่อระบบต่าง
ๆ\
Authentication กระบวนการพิสูจน์ตัวตนของผู้ใช้ เช่น Login Dashboard
หน้าจอสรุปข้อมูลสำหรับผู้ใช้หรือร้านค้า

Email Verification กระบวนการส่งอีเมลเพื่อยืนยันตัวตนหลังสมัคร สมาชิก\
FR Functional Requirement -- ความต้องการเชิง ฟังก์ชัน

─────────────────────────────────\
Template created for ENGCE301: Software Design and Development\
Rajamangala University of Technology Lanna\
อาจารย์ธนิต เกตุแก้ว\
Version 1.0 \| Academic Year 2024 -2025 Term Definition\
Hash กระบวนการแปลงข้อมูล (เช่น รหัสผ่าน) ให้เป็น
รูปแบบที่ไม่สามารถย้อนกลับได้\
JWT JSON Web Token -- Token ที่ใช้สำหรับยืนยัน สิทธิ์ผู้ใช้ ( Session
Token)\
Menu Item รายการอาหารที่ร้านค้าเพิ่มในระบบ\
NFR Non-Functional Requirement -- ความ ต้องการที่ไม่ใช่ฟังก์ชัน เช่น
ความปลอดภัย ความเร็ว\
Order Status สถานะของคำสั่งซื้อ (รอรับ, กำลังทำ , เสร็จแล้ว ฯลฯ) Payment
Gateway บริการกลางสำหรับตรวจสอบและประมวลผลการ ชำระเงิน\
PDPA กฎหมายคุ้มครองข้อมูลส่วนบุคคลของไทย\
Reservation การจองโต๊ะในร้านอาหาร\
Session สถานะการเข้าใช้งานของผู้ใช้ เช่น ขณะล็อกอิน\
Stakeholder บุคคลที่เกี่ยวข้องหรือมีผลกระทบต่อระบบ\
Student ID รหัสนักศึกษาที่ใช้เป็นตัวตนหลักในการ ลงทะเบียน\
Token ข้อมูลที่ใช้แทนการเข้าสู่ระบบเพื่อเข้าถึง API UI User Interface --
ส่วนที่ผู้ใช้โต้ตอบกับระบบ เช่น ปุ่ม หน้าจอ ฟอร์ม\
User Authentication โมดูลการลงทะเบียนและเข้าสู่ระบบของผู้ใช้\
Validation การตรวจสอบความถูกต้องของข้อมูลที่ป้อน เช่น\
Email Format หรือ Password Strength