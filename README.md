// basic-code
#include <stdio.h>

int main() {
    int n, i;
    float sum = 0.0, average;

    printf("Enter the number of integers: ");
    scanf("%d", &n);

    if (n <= 0) {
        printf("Invalid number of integers.\n");
        return 1;
    }

    int arr[n];
    printf("Enter %d integers:\n", n);
    for (i = 0; i < n; i++) {
        printf("Element %d: ", i + 1);
        scanf("%d", &arr[i]);
        sum += arr[i];
    }

    average = sum / n;
    printf("The average is: %.2f\n", average);

    return 0;
}
