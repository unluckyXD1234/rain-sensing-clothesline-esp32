อุปกรณ์ที่ใช้ต่อวงจร
-ESP32 CH9102X 32pin
-Servo Motor SG90 x2 
-Breadboard MB-102 x2
-Rain Drop Module MH-RD
-USB-C BreakOut
-USB Type-C Arduino
-สายจัมเปอร์ ผู้-ผู้
ถ้าอยากต่อให้สายยาวขึ้นใช้
-สายจัมเปอร์ ผู้-เมีย
-สายจัมเปอร์ เมีย-เมีย
โปรแกรมที่ใช้ 
-Arduino IDE
ส่วนตัวบ้านและราวตากผ้าออกแบบตามใจเลย

วิธีต่อวงจร
1.นำ Breadboard ตัวที่ 1 มาถอดร่าง +- ข้างหนึ่งออกและเอามาต่อกับ Breadboard ตัวที่ 2
2.นำ ESP32 เสียบลง Breadboard
3.Rain Sensor Module
›VCC ต่อกับ 3V3 ของ ESP32
›GND ต่อกับ GND ของ ESP32
›AO ต่อกับ GPIO 34 ของ ESP32
4.เสียบตัวโมดูล Type-C Breakout ลงบน Breadboard
›VCC ต่อเข้าร่าง +
›GND ต่อเข้าร่าง -
5.
ต่อสายไฟเลี้ยง SG90 Servo ทั้ง 2 ตัว
5.1 Servo ตัวที่ 1 (ควบคุมราวตากผ้า)
›สายสีแดง ต่อเข้าร่าง +
›สายสีน้ำตาลหรือดำ ต่อเข้าร่าง -
›สายสีเหลือง ต่อเข้า GPIO 18 ของ ESP32
5.2 Servo ตัวที่ 2 (ควบคุมที่กันสาด)
›สายสีแดง ต่อเข้าร่าง +
›สายสีน้ำตาลหรือดำ ต่อเข้าร่าง -
›สายสีเหลือง ต่อเข้า GPIO 19 ของ ESP32
6.ตัวบ้านและราวตากผ้าออกแบบตามใจเลย

ส่วน Code สามารถ Copy แล้วไปเปิดใน Google เพิ่มดูไฟล์และ Copy code ใส่ 
Arduino IDE ได้เลย 
[แต่ก่อนใส่อย่าลืมลง 
BOARDS MANAGER : esp32 by Espressif Systems
LIBRARY MANAGER : ESP32Servo by Kevin]
