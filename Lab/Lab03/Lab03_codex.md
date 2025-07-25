## โจทย์
จงจัดโค้ดโปรแกรมต่อไปนี้ให้อยู่ในรูปแบบมาตรฐาน Codex และแก้ไข Bug ของโปรแกรม

## FIX CODE
```c++
#include <stdio.h>
#include <math.h>

int isPrime(int num) {
    if (num < 2)
        return 0;
    for (int i = 2; i <= sqrt(num); i++) {
        if (num % i == 0)
            return 0;
    }
    return 1;
}

int main() {
    int n;
    printf("Enter N : ");
    scanf("%d", &n);
    int arr[n];
    for (int i = 0; i < n; i++) {
        printf("Enter value[%d] : ", i);
        scanf("%d", &arr[i]);
    }

    printf("Index:  ");
    for (int i = 0; i < n; i++) {
        printf("%2d ", i);
    }
    
    printf("\n");
    printf("Array:  ");
    for (int i = 0; i < n; i++) {
        if (isPrime(arr[i]))
            printf("%2d ", arr[i]);
        else
            printf(" # ");
    }
    printf("\n");

    return 0;
}

```

## TEST CASE
### Input
<img width="333" height="205" alt="image" src="https://github.com/user-attachments/assets/caa25fc7-305b-455a-8277-96fc0aef22d7" />

### Output
<img width="347" height="44" alt="image" src="https://github.com/user-attachments/assets/f4fd8cc6-2782-49cd-8b5f-80d897f0a664" />

