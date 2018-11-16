# Homework 05
จงเขียนโปรแกรมควบคุมแผงหลอดไฟ LED
* หลอดไฟ LED มีทั้งหมด 10 หลอด
* ในการ เปิด/ปิด หลอดไฟจะต้องระบุตำแหน่งของหลอด

## เงื่อนไข
* สถานะเริ่มต้นของหลอดไฟ LED ทุกดวงคือปิดอยู่
* ตำแหน่งของหลอดไฟ LED ทั้ง 10 หลอดให้ระบุเป็น 1-9 และ A ตามลำดับจากซ้ายไปขวา
* หลอดไฟที่ถูกเลือก (ถ้ามันเปิดอยู่มันจะทำการปิด, ถ้ามันปิดอยู่มันจะทำการเปิด)

## ตัวอย่าง
ตัวอย่างด้านล่างนี้เป็นการทำงานทีละขั้นตอนตามลำดับ  
> `<<รอรับ input>>` เป็นการรอรับข้อมูลจาก keyboard
```
[ ] [ ] [ ] [ ] [ ] [ ] [ ] [ ] [ ] [ ]
Please choose LED to turn On/Off: <<รอรับ input>>
```

ทำการเลือกหลอดไฟ 4 แล้วกด enter

```
[ ] [ ] [ ] [!] [ ] [ ] [ ] [ ] [ ] [ ]
Please choose LED to turn On/Off: <<รอรับ input>>
```

ทำการเลือกหลอดไฟ A แล้วกด enter

```
[ ] [ ] [ ] [!] [ ] [ ] [ ] [ ] [ ] [!]
Please choose LED to turn On/Off: <<รอรับ input>>
```

ทำการเลือกหลอดไฟ 4 แล้วกด enter

```
[ ] [ ] [ ] [ ] [ ] [ ] [ ] [ ] [ ] [!]
Please choose LED to turn On/Off: <<รอรับ input>>
```

> Notes:  
Assume the data is input by console.

## Interface(s)
```
public interface IHomework05
{
    string DisplayLEDOnScreen(string ledNo);
}
```