# Lab-01  ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)

ข้อมูลชนิดตัวเลขจำนวนเต็ม สามารถนำไปใช้งานได้หลากหลาย เช่น การนับหรือแสดงจำนวน การกำหนดลำดับที่ การจัดลำดับ เป็นต้น ค่าที่ใส่ลงในตัวแปร เป็นได้ทั้งค่าบวก ค่าศูนย์ และค่าลบ (มีตัวแปรบางชนิดที่เก็บเฉพาะค่าบวกเพียงอย่างเดียว) การกำหนดค่าใดๆ ให้กับตัวแปร ทำได้โดยการใช้เครื่องหมาย =
การใช้เครื่องหมายคณิตศาสตร์กับตัวแปรจำนวนเต็ม สามารถใช้ได้ทุกเครื่องหมาย ได้แก่ +, -, *, / และ %

## 15. การใช้เครื่องหมายทางคณิตศาสตร์กับตัวแปรชนิดจำนวนเต็ม

👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
int a, b, c, d, e, f;
a = 1;
b = a + 6;
c = b - 3;
d = c * 2;
e = d / 2;
f = e % 2;
Console.WriteLine("a={0}", a);
Console.WriteLine("b={0}", b);
Console.WriteLine("c={0}", c);
Console.WriteLine("d={0}", d);
Console.WriteLine("e={0}", e);
Console.WriteLine("f={0}", f);
```

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/a0aaa8a0-aac8-47e7-bc5f-c5328b597c1e)
โปรแกรมมีการดำเนินการทางคณิตระหว่างตัวแปร ด้วยการ บวก ลบ คูณ หาร 


## 16. หาค่าจากสมการทางคณิตศาสตร์

กำหนด ```a = 10, b = 20, x = 5, y = 2``
👉 ให้เขียนโปรแกรมเพื่อหาผลลัพธ์ของสมการต่อไปนี้

1. `a+b`
2. `x-b`
3. `x*b`
4. `y/a`
5. `b%y`
6. `y+10%x`
7. `a/3*5`
8. `9/2*a`
9. `y%8`
10. `100*x+y%2-a`
     ### ![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/af7cc23c-2259-4281-bae3-65a2712dfd0d)



## ชนิดข้อมูลเลขทศนิยม (Floating Point and Decimal Types)

ตัวเลขจำนวนทศนิยม มักจะใช้ในการคำนวณทางวิทยาศาสตร์ เนื่องจากค่าในวิทยาศาสตร์ต้องการความละเอียดสูง หรือมีค่าสูงมากกว่าที่เลขจำนวนเต็มจะเก็บได้

### ตัวอย่างการแก้ปัญหาทางวิทยาศาสตร์

ระยะทางจากดาวอาทิตย์ถึงโลกคือ 93,000,000 ไมล์ เรียกว่า 1 A.U. (Astronomical Unit)
ความเร็วในการเดินทางของแสงคือ 186,000 ไมล์ต่อวินาที
ระยะทาง 1 ไมล์ คิดเป็น 1.609344 กิโลเมตร
ให้เขียนโปรแกรมหาระยะทางในการเดินทางของแสง ในหน่วยกิโลเมตรต่อวินาทีและเวลาในการเดินทางของแสงจากดวงอาทิตย์มายังโลก

## 17.  โปรแกรมคำนวณระยะทางและเวลาของแสงจากดวงอาทิตย์ถึงโลก

👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
const double lightSpeed = 186000d;   // miles per second
Console.WriteLine("Light speed = {0} Mile Per second", lightSpeed);
const double mileTokm = 1.609344;
Console.WriteLine("Light speed = {0} km Per second", lightSpeed*mileTokm);
const double SunToEarthDistance =  93000000d ;  // miles
Console.WriteLine("SunToEarthDistance = {0} km", SunToEarthDistance * mileTokm);
double SunToEarthTimeOfLight = SunToEarthDistance / lightSpeed;  // miles
Console.WriteLine("SunToEarthTimeOfLight = {0} seconds", SunToEarthTimeOfLight);
Console.WriteLine("SunToEarthTimeOfLight = {0} minutes", SunToEarthTimeOfLight/60d);
```

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/2453e121-6d33-4c9b-8c5f-9a800a8308be)
โปรแกรมแสดงค่าความเร็วของแสง ความเร็วของแสง ระยะระหวว่างดวงอาทิตย์ คำนวณและแสดงเวลาที่แสงใช้เดินทาง แสดงเวลาที่แสงใช้เดินทางจากดวงอาทิตย์ ดังนั้นโค้ดนี้จะเป็นการแก้ปัญหาทางวิทยาศาสตร์ มีการกำหนดค่าคงที่ และแสดงหาผลลัพธ์



👷 คำสั่ง ให้เขียนโปรแกรมคำนวณค่าเพื่อเติมลงในช่องว่างในตาราง
ตารางที่ 1 ระยะทางจากดวงอาทิตย์ถึงดาวเคราะห์ต่างๆ

| ดาวเคราะห์ | ระยะทางจากดวงอาทิตย์ | ระยะทางในหน่วย A.U. | เวลาของแสง (นาที)
|---|---|---|---|
| Mercury | 57,910,000 km | 0.387098 |3.196294|
| Venus | 108,200,000 km | 0.723332| 6.003901|
| Earth | 149,600,000 km | 1.000000| 8.306696|
| Mars | 227,940,000 km | 1.523660|12.686664|
| Jupiter |  778,330,000 km | 5.204979|43.335805|
| Uranus | 2,873,550,000 km | 19.218472 | 159.954844|
| Neptune | 4,501,000,000 km |30.047860 | 249.650381|
| Pluto | 5,945,900,000 km | 39.810424 | 330.582599|


```csharp
using System;

class Program
{
    static void Main()
    {
        const double lightSpeed = 299792; // km per second
        const double auToKm = 149600000; // 1 astronomical unit (A.U.) = 149,600,000 kilometer 
        double[] distances = { 57910000, 108200000, 149600000, 227940000, 778330000, 2873550000, 4501000000, 5945900000 };
        Console.WriteLine("|  ดาวเคราะห์  | ระยะทางใน A.U. | เวลาของแสง (นาที) |");
        Console.WriteLine("|---------------|-------------------|-----------------------|");
        for (int i = 0; i < distances.Length; i++)
        {
            double distanceInAu = distances[i] / auToKm;
            double lightTimeInMinutes = distances[i] / lightSpeed / 60;

            Console.WriteLine("| {0,-13} | {1,17:F6} | {2,20:F6} |", GetPlanetName(i), distanceInAu, lightTimeInMinutes);
        }
    }
    static string GetPlanetName(int index)
    {
        string[] planetNames = { "Mercury", "Venus", "Earth", "Mars", "Jupiter", "Uranus", "Neptune", "Pluto" };
        return planetNames[index];
    }
}
```



 คลาส Math ในภาษา C# มีคลาสที่เป็นตัวช่วยคำนวณทางคณิตศาสตร์ ที่ช่วยให้เราสามารถคำนวณฟังก์ชันพื้นฐานได้ อย่างรวดเร็ว ไม่ต้องพัฒนาโปรแกรมเพิ่มเติมด้วยเอง นั่นคือคลาส Math ฟังก์ชันทางคณิตศาสตร์ที่ใช้บ่อยๆ สามารถดูรายละเอียดทั้งหมดได้จาก `system.math`

 
## 20.  โปรแกรมพล็อตรูป sine wave บนหน้าจอ

👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
for (float i = 0; i < Math.PI * 2.0F; i += 0.3F)
{
    Console.WriteLine("The sine of {0,10:F} = {1,-10:F6}" + spaces(Math.Sin(i)) + "*", i, Math.Sin(i));
}
string spaces(double val)
{
    string SpaceString = new String(' ', ((int)(val * 10.0)) + 10);
    return SpaceString;
}
```

หมายเหตุ ในการเขียนโปรแกรมภาษา C# .NET6.0 ที่ใช้ template แบบใหม่ เราก็ยังคงสามารถสร้าง function ใช้งานได้ตามปกติ (แต่จะไม่ครอบคลุม feature ทั้งหมดใน OOP )

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/a799c486-bb92-48ce-802b-bbb792a38634)
แสดงค่าและจำนวนช่องว่าวที่เพิ่มเข้าไป โดยที่แต่ละค่าจะถูกจัดหน้าให้อยู่ในคอลัมน์ด้วยช่องว่างที่สร้างขึ้น
  
