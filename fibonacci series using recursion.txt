#include <stdio.h>
int fibonacci(int num);

int main() {
    int num, i;

    printf("Enter the number of terms in the Fibonacci series: ");
    scanf("%d", &num);

    if (num < 1) {
        printf("Number of terms should be greater than or equal to 1.\n");
        return 1;
    }

    printf("Fibonacci series: ");
    for (i = 0; i < num; i++) {
        printf("%d ", fibonacci(i));
    }

    printf("\n");

    return 0;
}

int fibonacci(int num) {
    if (num == 0) {
        return 0;
    } else if (num == 1) {
        return 1;
    } else {
        return fibonacci(num - 1) + fibonacci(num - 2);
    }
}
