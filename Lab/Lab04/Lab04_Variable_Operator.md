## โจทย์
เขียนโปรแกรมภาษาซีเพื่อรับข้อมูลพนักงานของบริษัทซอร์ฟแวร์ โดยรับข้อมูล รหัสประจำตัวพนักงาน , จำนวนชั่วโมงที่ทำงาน , รายได้ต่อชั่วโมง จากนั้นให้แสดงข้อมูลเลขประจำตัวพนักงาน พร้อมกับรายได้ทั้งหมดที่หนักงานจะได้รับทั้งหมด

## FIX CODE
```c++
#include <stdio.h>

float workt = 0;
float Salaryt = 0;
float salary = 0;
char id[11];

int main() {
    printf("Input the Employees ID (Max. 10 chars) : ");
    scanf("%10s", id);

    printf("Input the working hrs : ");
    scanf("%f", &workt);

    printf("Salary amount/hr : ");
    scanf("%f", &Salaryt);

    salary = workt * Salaryt;

    printf("----------------------------\n");
    printf("Expected Output :\n");
    printf("Employees ID = %s\n", id);
    printf("Salary = U$ %.2f\n", salary);

    return 0;
}
```

## TEST CASE 1
### Input
<img width="410" height="69" alt="image" src="https://github.com/user-attachments/assets/ebae612c-82fa-4935-90dc-6baac1fcc5ac" />

### Output
<img width="250" height="67" alt="image" src="https://github.com/user-attachments/assets/80c04d3a-5254-4e89-bfc5-cac47c613c2a" />


## TEST CASE 2
### Input
<img width="488" height="65" alt="image" src="https://github.com/user-attachments/assets/915b8738-4cf6-4fec-bdb7-153a35ceff10" />

### Output
<img width="329" height="70" alt="image" src="https://github.com/user-attachments/assets/94d91324-54bb-4631-85a1-a271f5c0f5f7" />

