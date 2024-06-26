# Lab-01 การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ

ตัวแปรชนิด boolean มักจะถูกใช้เป็นที่เก็บผลที่เกิดจากการดำเนินการทางตรรกะ เช่น AND, OR, NOT เป็นต้น ซึ่งการดำเนินการทางตรรกะจะมีตารางความจริง เป็นตัวบอกผลในการดำเนินการของตัวดำเนินการต่างๆ ดังตัวย่าง

### ตัวดำเนินการ AND

Y = A AND B

| A | B | Y |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

### ตัวดำเนินการ OR

Y = A OR B

| A | B | Y |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

### ตัวดำเนินการ NOT

Y = NOT A

| A | Y |
|--|--|
| 0 | 1 |
| 1 | 0 |

ตัวดำเนินการในภาษา C#
ใช้เครื่องหมายต่างๆ ดังต่อไปนี้

| การดำเนินการ | เครื่องหมาย |
|------------|-----------|
| Logical AND | & |
| Logical XOR | ^ |
| Logical OR | \| |

## 14. การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ

ตัวอย่างภาษา C# ต่อไปนี้เป็นการพิมพ์ตารางความจริงออกทางหน้าจอ
👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
bool A, B,Y;
Console.WriteLine("      Y = A AND B");
Console.WriteLine("-----------------------");
Console.WriteLine("   A      B\t|  Y");
Console.WriteLine("-----------------------");
A = false; B = false; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A,B,Y);
A = false; B = true; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
A = true; B = false; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
A = true; B = true; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
Console.WriteLine("-----------------------");
```

➢ รันโปรแกรมและบันทึกผล

 ![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/0db8b484-a69d-47df-a68c-1d047dd48bd0)
code ทำการคำนวณผลลัพธ์ของการดำเนินการทางตรรกะ AND ระหว่างตัวแปร A,Bแสดงออกผลลัพธ์ออกมาเป็นตาราง 
👷 จากจ้อ 14 ให้เขียนโปรแกรมเพื่อสร้างตารางความจริงของลอจิกดังต่อไปนี้

1. `AND`![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/21259556-ee34-4d88-8512-ee972e228fee)

2. `OR` ![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/bedfdca3-5e32-4e91-b120-fc29de2c75c6)

3. `NOT`![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/789fbe70-da62-4eef-83bc-70e362464bce)

4. `NAND`![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/ba5dcfc7-27e5-401b-ac25-eda2f7eefd93)

5. `NOR`![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/15dd6866-f2aa-4548-b453-4935c0e29eca)

6. `Exclusive OR`![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/bdcac734-71e2-4f7f-8ff6-b8f4f2f85203)



## [ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)](./Lab-01-part-15.md)
