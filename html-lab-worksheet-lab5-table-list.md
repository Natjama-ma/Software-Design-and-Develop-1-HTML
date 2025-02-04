# ใบงานการทดลอง HTML

## การทดลองที่ 5: การสร้างตารางและรายการ
### วัตถุประสงค์
- เรียนรู้การสร้างตารางข้อมูล
- เรียนรู้การสร้างรายการแบบต่างๆ

### ขั้นตอนการทดลอง
1. สร้างไฟล์ tablelist.html ดังตัวอย่าง:
```html
<table border="1">
    <thead>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Row 1, Cell 1</td>
            <td>Row 1, Cell 2</td>
        </tr>
        <tr>
            <td>Row 2, Cell 1</td>
            <td>Row 2, Cell 2</td>
        </tr>
    </tbody>
</table>
```

### คำอธิบายเพิ่มเติม
- `<table>` กำหนดขอบเขตของตาราง
- `<thead>` สำหรับส่วนหัวตาราง
- `<tbody>` สำหรับเนื้อหาตาราง
- `<tr>` แทนแถว
- `<th>` แทนเซลล์หัวตาราง
- `<td>` แทนเซลล์ข้อมูล

2. การสร้างรายการ โดยเพิ่มเติม Code ในไฟล์ tablelist.html :
```html
<ul>
    <li>Unordered item 1</li>
    <li>Unordered item 2</li>
</ul>

<ol>
    <li>Ordered item 1</li>
    <li>Ordered item 2</li>
</ol>

<dl>
    <dt>Term 1</dt>
    <dd>Definition 1</dd>
    <dt>Term 2</dt>
    <dd>Definition 2</dd>
</dl>
```

### คำอธิบายเพิ่มเติม
- `<ul>` สำหรับรายการแบบไม่เรียงลำดับ
- `<ol>` สำหรับรายการแบบเรียงลำดับ
- `<dl>` สำหรับรายการแบบคำจำกัดความ
- `<li>` แทนรายการแต่ละรายการ

### แบบฝึกหัด
1. สร้างตารางแสดงข้อมูลส่วนตัว
2. สร้างรายการเมนูอาหาร

- ภาพผลลัพธ์:
[วางภาพ screenshot ที่นี่]

![image](https://github.com/user-attachments/assets/4c0a1376-1709-49d8-94d4-20197380214b)

[วางโค้ด HTML ที่นี่]
```<!DOCTYPE html>
<html lang="th"> 
<head>
    <meta charset="UTF-8">
    <title>หน้าหลัก</title>
    <style>
        table {
          width: 50%;       /* กำหนดความกว้างเป็น 70% ของ container */
          height: 100px;    /* กำหนดความสูงเป็น 300px */
          border-collapse: collapse;
        }
        th, td {
          border: 1px solid black;
          padding: 1px;
          text-align: center;
        }
      </style>
</head>
<body>
    <h1>ข้อมูลส่วนตัว</h1>
    <table border="1">
    <thead>
        <tr><strong>
            <th>ข้อมูลส่วนตัว</th>
            <th>รายละเอียด</th>
            </strong>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>ชื่อ-สกุล</td>
            <td>นัจญมา จันทร์ชู</td>
        </tr>
        <tr>
            <td>รหัสนักศึกษา</td>
            <td>67030110</td>
        </tr>
        <tr>
            <td>อายุ</td>
            <td>18</td>
        </tr>
        <tr>
            <td>มหาวิทยาลัย</td>
            <td>สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง</td>
        </tr>
        <tr>
            <td>คณะ</td>
            <td>ครุศาสตร์อุตสาหกรรมและเทคโนโลยี</td>
        </tr>
        <tr>
            <td>สาขาวิชา</td>
            <td>เทคโนโลยีคอมพิวเตอร์</td>
        </tr>
        <tr>
            <td>ที่อยู่</td>
            <td>จังหวัดระนอง</td>
        </tr>
        <tr>
            <td>หมายเลขโทรศัพท์</td>
            <td>065-484-xxxx</td>
        </tr>
        <tr>
            <td>อีเมล</td>
            <td>67030110@kmitl.ac.th</td>
        </tr>
    </tbody>
</table><br><hr>
<h1>รายการเมนูอาหาร</h1>
<table>
    <thead>
        <tr><strong>
            <th>เมนูอาหาร</th>
            <th>ราคา (บาท)</th>
            </strong>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>ข้าวผัดไก่/กุ้ง/เนื้อ</td>
            <td>50</td>
        </tr>
        <tr>
            <td>ผัดกะเพราไก่/กุ้ง/เนื้อ</td>
            <td>65</td>
        </tr>
        <tr>
            <td>ต้มยำกุ้ง</td>
            <td>65</td>
        </tr>
        <tr>
            <td>แกงไตปลา</td>
            <td>60</td>
        </tr>
        <tr>
            <td>แกงส้มกุ้ง/ปลา</td>
            <td>65</td>
        </tr>
        <tr>
            <td>แกงหน่อไม้</td>
            <td>60</td>
        </tr>
        <tr>
            <td>แกงเขียวหวานไก่/ลูกชิ้น/ปลา</td>
            <td>70</td>
        </tr>
        <tr>
            <td>ปลาสามรส</td>
            <td>60</td>
        </tr>
    </tbody>
</table>
</body>
</html>
```
