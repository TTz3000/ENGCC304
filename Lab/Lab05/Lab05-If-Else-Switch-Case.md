## โจทย์
ผู้ใช้กรอกค่า "คะแนนดิบ" เข้ามาในระบบเพื่อต้องการตรวจสอบเกรดในรายวิชา Programming ซึ่งมีเกณฑ์การให้คะแนนคือ 
<br />F อยู่ในช่วงคะแนนน้อยกว่า 50 , 
<br />D อยู่ในช่วงระหว่าง 50 ถึง 55 , 
<br />D+ อยู่ในช่วงระหว่าง 55 ถึง 60 , 
<br />C อยู่ในช่วงระหว่าง 60 ถึง 65 , 
<br />C+ อยู่ในช่วงระหว่าง 65 ถึง 70 , 
<br />B อยู่ในช่วงระหว่าง 70 ถึง 75 , 
<br />B+ อยู่ในช่วงระหว่าง 75 ถึง 80 , 
<br />A อยู่ในช่วงคะแนนมากกว่า 80 ขึ้นไป 
<br /><br />(กำหนดให้ข้อนี้ใช้คำสั่ง if else ได้เท่านั้น)

## FIX CODE
```c++
#include <stdio.h>

int main() {
    int score = 0;

    printf("Enter your Score : ");

    if (scanf("%d", &score) != 1) {
        printf("Please enter number only.\n");
        return 0;
    }

    if (score > 100) {
        printf("Please don't enter a number over 100!!!\n");
    } else if (score < 0) {
        printf("Please don't enter a number below 0!!!\n");
    } else if (score >= 80) {
        printf("A !\n");
    } else if (score >= 75) {
        printf("B+ !\n");
    } else if (score >= 70) {
        printf("B !\n");
    } else if (score >= 65) {
        printf("C+ !\n");
    } else if (score >= 60) {
        printf("C !\n");
    } else if (score >= 55) {
        printf("D+ !\n");
    } else if (score >= 50) {
        printf("D !\n");
    } else {
        printf("F !\n");
    }

    return 0;
}
```

## TEST CASE
### Input - 
<img width="218" height="22" alt="image" src="https://github.com/user-attachments/assets/9251bf14-a7fc-413e-859a-6a64716ea915" />

### Output
<img width="47" height="23" alt="image" src="https://github.com/user-attachments/assets/18c51934-35b8-459e-a82b-04405746cf50" />

## TEST CASE
### Input - Output
<img width="211" height="44" alt="image" src="https://github.com/user-attachments/assets/a773e245-edf0-4cde-883b-4992d55fb9ad" />

## TEST CASE
### Input - Output
<img width="223" height="47" alt="image" src="https://github.com/user-attachments/assets/79fb42d4-0483-41d4-97cd-2e2d5b7c7801" />

## TEST CASE
### Input - Output
<img width="231" height="49" alt="image" src="https://github.com/user-attachments/assets/94d6441c-d02b-4dff-97a8-ddb30b57d179" />

## TEST CASE
### Input - Output
<img width="282" height="50" alt="image" src="https://github.com/user-attachments/assets/8ead21f3-ddc4-4809-8143-6824a8cd5c6e" />


