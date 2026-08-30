# Coffee Shop Business & Queue System

## โปรเจกต์นี้เป็นส่วนหนึ่งของรายวิชา SC612104 Essential Data Science

โปรเจกต์จำลองระบบร้านกาแฟตั้งแต่การรับออเดอร์ คำนวณราคา ชำระเงิน
ส่งข้อมูลไปยัง KDS เรียกคิว และส่งมอบสินค้า พร้อมสร้างข้อมูลจำลอง
เพื่อนำไปวิเคราะห์ด้วย Pandas, SQLite SQL และ BigQuery

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kunphat510214-netizen/Project-6-coffee-shop-/blob/main/Coffee_Shop.ipynb)

## Repository นี้ประกอบด้วย

- Source Code และผลการวิเคราะห์ทั้งหมดใน Jupyter Notebook:
  [Link](./Coffee_Shop.ipynb)
- ไฟล์กราฟสรุปผลการวิเคราะห์:
  [Link](./coffee_analysis.png)
- ฐานข้อมูล SQLite จำนวน 3 ตาราง ได้แก่ orders, members และ
  order_events:
  [Link](./coffee_shop.db)
- โฟลเดอร์เก็บไฟล์ CSV:
  [Link](./data)

### ไฟล์ข้อมูลจำลอง

- ข้อมูลออเดอร์ 300 รายการ:
  [Link](./data/coffee_orders.csv)
- ข้อมูลสมาชิก 60 รายการ:
  [Link](./data/members.csv)
- ประวัติการเปลี่ยนสถานะออเดอร์ 1,200 รายการ:
  [Link](./data/order_events.csv)

### ไฟล์ผลสรุปจาก BigQuery

- ผลการวิเคราะห์ประสิทธิภาพของเมนู:
  [Link](./data/summary_menu_performance.csv)
- ผลการวิเคราะห์ตามประเภทลูกค้า:
  [Link](./data/summary_customer_type.csv)
- ผลการวิเคราะห์ตามประเภทเครื่องดื่ม:
  [Link](./data/summary_drink_type.csv)

## ความสามารถหลักของระบบ

1. ออกแบบระบบด้วย 3 Classes ได้แก่ Member, DrinkOrder และ QueueSystem
2. จำลองธุรกรรมร้านกาแฟจำนวน 300 ออเดอร์ด้วย Loop
3. บันทึกข้อมูลเป็น CSV และฐานข้อมูล SQLite
4. วิเคราะห์ข้อมูลด้วย Pandas โดยใช้ describe(), info(), groupby(), agg()
   และ sort_values()
5. วิเคราะห์ด้วย SQL โดยใช้ SELECT, WHERE, ORDER BY, GROUP BY,
   Aggregate Functions และ JOIN
6. แสดงผลด้วยกราฟ 3 รูปแบบ พร้อมสรุปข้อค้นพบทางธุรกิจ

## สมาชิกและบทบาทหน้าที่

1. น.ส.กุลภัสสร์ เคล้าโนนคร้อ 683020239-7
   (ฝ่ายพัฒนาระบบ Source Code)
2. น.ส.อรปรีญา เฉิดไธสง 683020599-7
   (ฝ่ายจำลอง และสร้างฐานข้อมูล)
3. นายธนกร สมหาญ 683020246-0
   (ฝ่ายวิเคราะห์ และสรุปผลข้อมูล)
4. นางสาวณัฐฐธิดา พันสวัสดิ์ 683020243-6
   (ฝ่ายพัฒนาระบบ Source Code)

## เครื่องมือที่ใช้

- Python
- Pandas
- SQLite
- Google BigQuery
- Matplotlib
- Google Colab
