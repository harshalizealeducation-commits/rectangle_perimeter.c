# rectangle_perimeter.c

#include <stdio.h>

int main() {
    float units, bill;

    printf("Enter electricity units: ");
    scanf("%f", &units);

    if (units < 0) {
        printf("Invalid units\n");
    } else {
        if (units <= 100)
            bill = units * 2;
        else if (units <= 200)
            bill = 200 + (units - 100) * 3;
        else
            bill = 500 + (units - 200) * 5;

        printf("Electricity Bill = Rs. %.2f\n", bill);
    }

    return 0;
}
