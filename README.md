# Ravindrababu
Project Test

วัดอุณภูมิ และเก็บข้อมูลลงใน Firebase และแสดงผลบน phpmyadmin มี LED แสดงสถานะการทำงาน มีการแจ้งเตือนอุณภูมิความชื้นเข้าไลน์เมื่อต่ำกว่าที่กำหนดได้

อุปกรณ์ที่ใช้งาน
ESP8266 LCD16*2 LEDRGB1 DHT22

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
