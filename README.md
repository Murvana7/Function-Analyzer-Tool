#include <stdio.h>
#include <math.h>

int main() {
    int choice;
    double x, result;

    printf("=== Derivative Calculator ===\n");
    printf("1. d/dx (x^3)\n");
    printf("2. d/dx (sin x)\n");
    printf("3. d/dx (cos x)\n");
    printf("4. d/dx (exp x)\n");
    printf("Choose function (1-4): ");
    scanf("%d", &choice);

    printf("Enter value of x: ");
    scanf("%lf", &x);

    switch (choice) {
        case 1:
            result = 3 * x * x;
            printf("Derivative = %.4f\n", result);
            break;

        case 2:
            result = cos(x);
            printf("Derivative = %.4f\n", result);
            break;

        case 3:
            result = -sin(x);
            printf("Derivative = %.4f\n", result);
            break;

        case 4:
            result = exp(x);
            printf("Derivative = %.4f\n", result);
            break;

        default:
            printf("❌ Invalid choice\n");
    }

    return 0;
}
