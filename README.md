# Coffee Shop Business & Queue System

## โปรเจกต์นี้เป็นส่วนหนึ่งของรายวิชา SC612104 Essential Data Science

โปรเจกต์จำลองระบบร้านกาแฟตั้งแต่การรับออเดอร์ คำนวณราคา ชำระเงิน
ส่งข้อมูลไปยัง KDS เรียกคิว และส่งมอบสินค้า พร้อมสร้างข้อมูลจำลอง
เพื่อนำไปวิเคราะห์ด้วย Pandas, SQLite SQL และ BigQuery

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kunphat510214-netizen/Final-Final/blob/main/Coffee_Shop.ipynb)

## Repository นี้ประกอบด้วย

- Source Code และผลการวิเคราะห์ทั้งหมดใน Jupyter Notebook:
  [Coffee_Shop.ipynb](./Coffee_Shop.ipynb)
- ไฟล์กราฟสรุปผลการวิเคราะห์:
  [coffee_analysis.png](./coffee_analysis.png)
- ฐานข้อมูล SQLite จำนวน 3 ตาราง ได้แก่ orders, members และ
  order_events:
  [coffee_shop.db](./coffee_shop.db)
- โฟลเดอร์เก็บไฟล์ CSV:
  [data](./data)

### ไฟล์ข้อมูลจำลอง

- ข้อมูลออเดอร์ 300 รายการ:
  [coffee_orders.csv](./data/coffee_orders.csv)
- ข้อมูลสมาชิก 60 รายการ:
  [members.csv](./data/members.csv)
- ประวัติการเปลี่ยนสถานะออเดอร์ 1,200 รายการ:
  [order_events.csv](./data/order_events.csv)

### ไฟล์ผลสรุปจาก BigQuery

- ผลการวิเคราะห์ประสิทธิภาพของเมนู:
  [summary_menu_performance.csv](./data/summary_menu_performance.csv)
- ผลการวิเคราะห์ตามประเภทลูกค้า:
  [summary_customer_type.csv](./data/summary_customer_type.csv)
- ผลการวิเคราะห์ตามประเภทเครื่องดื่ม:
  [summary_drink_type.csv](./data/summary_drink_type.csv)

## ความสามารถหลักของระบบ

1. ออกแบบระบบด้วย 3 Classes ได้แก่ Member, DrinkOrder และ QueueSystem
2. จำลองธุรกรรมร้านกาแฟจำนวน 300 ออเดอร์ด้วย Loop
3. บันทึกข้อมูลเป็น CSV และฐานข้อมูล SQLite
4. วิเคราะห์ข้อมูลด้วย Pandas โดยใช้ describe(), info(), groupby(), agg()
   และ sort_values()
5. วิเคราะห์ด้วย SQL โดยใช้ SELECT, WHERE, ORDER BY, GROUP BY,
   Aggregate Functions และ JOIN
6. แสดงผลด้วยกราฟ 3 รูปแบบ พร้อมสรุปข้อค้นพบทางธุรกิจ

## วิธีเปิดและรันโปรเจกต์

1. กดปุ่ม **Open in Colab** ด้านบน
2. เลือกเมนู Runtime → Run all
3. รอให้ระบบสร้างข้อมูล วิเคราะห์ SQL และแสดงกราฟจนเสร็จ
4. ตรวจสอบว่าแต่ละเซลล์ไม่มี Error ก่อนบันทึกหรือส่งงาน

> Notebook กำหนด random.seed(612104) จึงสร้างข้อมูลชุดเดิมเมื่อกด
> Run All ใหม่ ทำให้ผลวิเคราะห์สามารถทำซ้ำได้

## เครื่องมือที่ใช้

- Python
- Pandas
- SQLite
- Google BigQuery
- Matplotlib
- Google Colab
