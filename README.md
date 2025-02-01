#include <stdio.h>

int main() {
    // Declare variables
    float ricePrice, sugarPrice, oilPrice;
    int riceQuantity, sugarQuantity, oilQuantity;
    float subtotal, tax, total;

    // Get user input
    printf("Enter price of rice per unit: $");
    scanf("%f", &ricePrice);
    printf("Enter quantity of rice: ");
    scanf("%d", &riceQuantity);

    printf("Enter price of sugar per unit: $");
    scanf("%f", &sugarPrice);
    printf("Enter quantity of sugar: ");
    scanf("%d", &sugarQuantity);

    printf("Enter price of oil per unit: $");
    scanf("%f", &oilPrice);
    printf("Enter quantity of oil: ");
    scanf("%d", &oilQuantity);

    // Calculate subtotal
    subtotal = (ricePrice * riceQuantity) + (sugarPrice * sugarQuantity) + (oilPrice * oilQuantity);

    // Calculate tax
    tax = subtotal * 0.05;

    // Calculate total
    total = subtotal + tax;

    // Print results
    printf("\nSubtotal: $%.2f\n", subtotal);
    printf("Tax (5%%): $%.2f\n", tax);
    printf("Total: $%.2f\n", total);

    return 0;
}
