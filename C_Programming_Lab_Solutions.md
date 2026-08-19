# C Programming Lab: for Loop Practice Problems — Solutions

---

## 1. Print Multiplication Table

```c
#include <stdio.h>

int main() {
    int n;

    printf("Enter a number: ");
    scanf("%d", &n);

    for (int i = 1; i <= 10; i++) {
        printf("%d x %d = %d\n", n, i, n * i);
    }

    return 0;
}
```

---

## 2. Print Multiples of a Number

```c
#include <stdio.h>

int main() {
    int n;

    printf("Enter a number: ");
    scanf("%d", &n);

    printf("Multiples of %d between 1 and 100:\n", n);
    for (int i = 1; i <= 100; i++) {
        if (i % n == 0) {
            printf("%d\n", i);
        }
    }

    return 0;
}
```

---

## 3. Count Numbers Divisible by 3

```c
#include <stdio.h>

int main() {
    int count = 0;

    printf("Numbers divisible by 3 between 1 and 100:\n");
    for (int i = 1; i <= 100; i++) {
        if (i % 3 == 0) {
            printf("%d\n", i);
            count++;
        }
    }

    printf("Total count = %d\n", count);
    return 0;
}
```

---

## 4. Sum of Multiples of 5

```c
#include <stdio.h>

int main() {
    int sum = 0;

    for (int i = 1; i <= 100; i++) {
        if (i % 5 == 0) {
            sum += i;
        }
    }

    printf("Sum of multiples of 5 = %d\n", sum);
    return 0;
}
```

---

## 5. Sum of Squares

Find: 1² + 2² + 3² + ... + n²

```c
#include <stdio.h>

int main() {
    int n;
    long sum = 0;

    printf("Enter n: ");
    scanf("%d", &n);

    for (int i = 1; i <= n; i++) {
        sum += i * i;
    }

    printf("Sum of squares = %ld\n", sum);
    return 0;
}
```

---

## 6. Sum of Cubes

Find: 1³ + 2³ + 3³ + ... + n³

```c
#include <stdio.h>

int main() {
    int n;
    long sum = 0;

    printf("Enter n: ");
    scanf("%d", &n);

    for (int i = 1; i <= n; i++) {
        sum += i * i * i;
    }

    printf("Sum of cubes = %ld\n", sum);
    return 0;
}
```

---

## 7. Sum of Numbers in a Range

```c
#include <stdio.h>

int main() {
    int a, b, sum = 0;

    printf("Enter a and b: ");
    scanf("%d %d", &a, &b);

    // handle the case where a > b
    if (a > b) {
        int temp = a;
        a = b;
        b = temp;
    }

    for (int i = a; i <= b; i++) {
        sum += i;
    }

    printf("Sum from %d to %d = %d\n", a, b, sum);
    return 0;
}
```

---

## 8. Print Numbers with Their Squares

```c
#include <stdio.h>

int main() {
    int n;

    printf("Enter n: ");
    scanf("%d", &n);

    printf("Number\tSquare\n");
    for (int i = 1; i <= n; i++) {
        printf("%d\t%d\n", i, i * i);
    }

    return 0;
}
```
