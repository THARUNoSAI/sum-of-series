#include <stdio.h>

void calculate(int n, double *sum, double prev_factorial) {
    if (n == 0) {
        return;
    }
    double factorial = 1.0;
    for (int i = 1; i <= n; i++) {
        factorial *= i;
    }
    *sum += factorial / n;
    calculate(n - 1, sum, factorial);
}

int main() {
    int n;
    printf("Enter the value of n: ");
    scanf("%d", &n);

    double sum = 0.0;
    calculate(n, &sum, 1.0);

    printf("Sum of the series: %lf\n", sum);

    return 0;
}
