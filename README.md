# Basic-RecyclerView
แอพนี้แสดงการใช้  RecyclerView เพื่อแสดงรายการที่เลื่อนบนหน้าจอเมือถูกเลื่อนไป 
จะนำการแสดงผลนั้นกลับมาใช้ใหม่พร้อมข้อมูลชุดใหม่ ทำให้เกิดความลื่นไหลและประมวลผลได้ดีขึ้น
เริ่มต้นเปิดไฟล์ strings.xml แล้วเพิ่มชุดข้อมูลสตริงของคุณ

![Stringxml](https://user-images.githubusercontent.com/110089122/184409630-50ae7dc1-1618-4cca-bca3-c6a6613c632a.png)

จากนั้นให้สร้างแพ็คเกจชื่อว่า model ภายในแพ็คเกจ modelให้สร้าง ไฟล์ kolin file/class 
เพิ่มคีย์เวิร์ด data ก่อนคลาส โดยใช้ชื่อว่า Affirmationคลาส และเพิ่ม val เพื่อส่งผ่านข้อมูลสตริง ให้เป็นจำนวนเต็ม
![modelaff](https://user-images.githubusercontent.com/110089122/184410138-7c59ba34-7244-4066-87e5-bd26e35febf7.png)

![sentstringtoint](https://user-images.githubusercontent.com/110089122/184410282-73320b3f-6d1c-4240-8ec0-70fc66561edc.png)

จากนั้นให้สร้างแพ็คเกจชื่อ data ภายในจะสร้างไฟล์ kolin file/class ชื่อ Datasource จากนั้นให้สร้างฟังชั่นชื่อ loadAffirmation() เพื่อโหลดข้อมูลและ ส่งคืนเป็นข้อมูลสตริง
![datasour](https://user-images.githubusercontent.com/110089122/184410434-ba5a4c55-067a-4dde-9088-fb8ca2e6fe8b.png)

![loadreturn](https://user-images.githubusercontent.com/110089122/184410463-02187ca9-71c2-4503-aa10-408ffb81c0ce.png)

![loadreturn](https://user-images.githubusercontent.com/110089122/184410728-12d9e932-9092-4eca-b959-cac97ab393b4.png)

หลังจากนั้นมาที่ activity_main.xml และกำหนดให้ใช้ FrameLaout แทน แล้วค่อยส้ราง RecyclerView ดั่งภาพ
![activimain](https://user-images.githubusercontent.com/110089122/184411995-a1b89e14-0409-4cf7-b9ab-9b195ac0e928.png)

จากนั้นสร้างแพ็คเกจชื่อ adapter ภายในให้สร้างไฟล์ kolin file/class ชื่อว่า ItemAdapter ดั่งภาพ
![adapitem](https://user-images.githubusercontent.com/110089122/184413800-3bc66898-0d06-4542-afc3-614c4d6c3ab3.png)

![itemadap](https://user-images.githubusercontent.com/110089122/184412700-501f6535-40e6-41b0-b495-e6e54b95a9f8.png)
จากนั้นให้กด Control+i บน windows จะแสดงรายการ getItemcount()..oncreateViewHolder, onbindViewHolder เลือกทั้งหมดและคลิ๊ก Click OK
แล้วเพิ่มโค้ดดั่งในภาพ
![overi](https://user-images.githubusercontent.com/110089122/184413552-de991dd9-3110-42f6-997f-939c107ba3d7.png)

ผลลัพท์
![fins](https://user-images.githubusercontent.com/110089122/184414228-160b4030-29ae-4e27-bda1-034f52e3e36c.png)

จัดทำโดยใช้เรียนในวิชา Mobile Development for Android Platform
