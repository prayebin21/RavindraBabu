# Ravindrababu
Project Test

วัดอุณภูมิ และเก็บข้อมูลลงใน Firebase และแสดงผลบน phpmyadmin มี LED แสดงสถานะการทำงาน มีการแจ้งเตือนอุณภูมิความชื้นเข้าไลน์เมื่อต่ำกว่าที่กำหนดได้

อุปกรณ์ที่ใช้งาน
ESP8266 LCD16*2 LEDRGB1 DHT22

![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/create/DHT22.png)


  DHT22 เป็นเซ็นเซอร์ทีใช้การสื่อสารแบบ 1-Wire ทำให้ใช้สายเพียง 3 เส้นเท่านั้น แต่ที่ตัวเซ็นเซอร์มีขาทั้งหมด 4 ขา จะใช้งานเพียงขาที่ 1 เป็น VCC สามารถจ่ายไฟได้ตั้งแต่ 2.8 - 5.5V และขาที่ 2 เป็นขา DATA สำหรับส่งสัญญาณสื่อสารกับไมโครคอนโทรลเลอร์ ส่วนขาที่ 3 เป็นขาว่าง ขาที่ 4 เป็นขา GND
การต่ออุปกรณ์


การต่อวงจร DHT11 / DHT22 กับ Arduino ต่อตามรูปนี้

![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/create/1.png)

สำหรับการต่อวงจร DHT21 กับ Arduino ต่อตามนี้

สายสีดำ -> Gnd
สายสีแดง -> 5 Vcc
สายสีเหลือง -> 2 (สาย ข้อมูล)
ต่อ R 4.7K คร่อมสายสีแดงกับสายสีเหลือง

ฟังก์ชั่นการทำงาน DHT22

![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/create/code.png)

หน้าต่างโค้ดโปรแกรม ที่เขียนบน Arduino

![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/Pic/Screenshot_1.png)

หน้าต่างแสดงผลการทำงานของ DHT22

![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/Pic/20727206_1507666329297025_782399047_o.jpg)

การต่ออุปกรณ์

![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/Pic/20067709_1407499735994460_691601708_n.png)
![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/Pic/20746873_1507662849297373_183159908_o.jpg)
![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/Pic/20747539_1507662815964043_1074973169_o.jpg)
![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/Pic/20747595_1507662782630713_1423495890_o.jpg)


การส่งสถานะการทำงานเข้าสู้ Line Notify

-เริ่มต้นประกาศ define Line Token แล้วนำรหัส Token จาก Line Notify

![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/Line/token.png)

-โค้ดการส่งค่า

![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/Line/send%20to%20line.png)

-เงื่อนไขในการส่งค่าเข้าสู่ Line

![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/Line/change.png)

-ตัวอย่างการส่งข้อมูล

![alt text](https://github.com/prayebin21/Ravindrababu/blob/master/Pic/20771564_1507666802630311_320918708_o.jpg)
