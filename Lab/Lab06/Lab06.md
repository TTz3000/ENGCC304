## โจทย์
จงเขียนโปรแกรมรับค่าตัวเลขจากผู้ใช้ ใส่ไว้ในตัวแปร N และทำการแสดงข้อมูลดังเงื่อนไขต่อไปนี้
<br />- หากผู้ใช้กรอกเลขคี่ ให้โปรแกรมแสดงลำดับตัวเลขตั้งแต่ 1 ถึง N และให้แสดงเฉพาะตัวเลขคี่เท่านั้น
<br />- หากผู้ใช้กรอกเลขคู่ ให้โปรแกรมแสดงลำดับตัวเลขตั้งแต่ N ถึง 0 และให้แสดงเฉพาะตัวเลขคู่เท่านั้น


## FIX CODE
```c++
#include <stdio.h>

int main() {
    int num = -1;

    printf("Enter Value : ");
    scanf("%d" , &num);

    int num1 = num;
    num1 = num1 % 2;

    int i = 0;

    if( num < 0 ){
        printf("Pleses enter only Number!");
        return 0 ;
    }

    printf("Series : ");

    if( num1 != 0 ) {
        for( i = 1 ; i <= num ; i += 2 ) {
            printf("%d " , num1);
            num1 += 2;
        }
    } else {   
        num1 = num;
        for( i = 0 ; i <= num ; i += 2 ) {
            printf("%d " , num1);
            num1 -= 2;
        }
    } 

    return 0;
}
```

## TEST CASE
### Even Number
### Input & Output
<img width="264" height="48" alt="image" src="https://github.com/user-attachments/assets/bf6092f1-2142-4fc4-88af-cb4b50e21a3f" />

### Odd Number
### Input & Output
<img width="318" height="48" alt="image" src="https://github.com/user-attachments/assets/64bd3301-57d0-48c8-a0c9-a5601f6a1f5b" />

