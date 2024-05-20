#include <stdio.h>

int main()
{
    int choice;
    float value;

    while (1)
    {
        printf("\n*Welcome to our Conversion Program*\nPlease choose the any one option\n");
        printf("1. Length Conversion\n");
        printf("2. Weight Conversion\n");
        printf("3. Temperature Conversion\n");
        printf("4. Quit\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);

        switch (choice)
        {
        case 1:
            printf("Length Conversion\n");
            printf("1. Kilometers to Miles\n");
            printf("2. Miles to Kilometers\n");
            printf("Enter your choice: ");
            scanf("%d", &choice);

            switch (choice)
            {
            case 1:
                printf("Enter value in kilometers: ");
                scanf("%f", &value);
                printf("%.2f kilometers is equal to %.2f miles\n", value, value * 0.621371);
                break;
            case 2:
                printf("Enter value in miles: ");
                scanf("%f", &value);
                printf("%.2f miles is equal to %.2f kilometers\n", value, value / 0.621371);
                break;
            default:
                printf("Invalid choice\n");
            }
            break;
        case 2:
            printf("Weight Conversion\n");
            printf("1. Kilograms to Pounds\n");
            printf("2. Pounds to Kilograms\n");
            printf("Enter your choice: ");
            scanf("%d", &choice);

            switch (choice)
            {
            case 1:
                printf("Enter value in kilograms: ");
                scanf("%f", &value);
                printf("%.2f kilograms is equal to %.2f pounds\n", value, value * 2.20462);
                break;
            case 2:
                printf("Enter value in pounds: ");
                scanf("%f", &value);
                printf("%.2f pounds is equal to %.2f kilograms\n", value, value / 2.20462);
                break;
            default:
                printf("Invalid choice\n");
            }
            break;
        case 3:
            printf("Temperature Conversion\n");
            printf("1. Celsius to Fahrenheit\n");
            printf("2. Fahrenheit to Celsius\n");
            printf("Enter your choice: ");
            scanf("%d", &choice);

            switch (choice)
            {
            case 1:
                printf("Enter value in Celsius: ");
                scanf("%f", &value);
                printf("%.2f Celsius is equal to %.2f Fahrenheit\n", value, (value * 9 / 5) + 32);
                break;
            case 2:
                printf("Enter value in Fahrenheit: ");
                scanf("%f", &value);
                printf("%.2f Fahrenheit is equal to %.2f Celsius\n", value, (value - 32) * 5 / 9);
                break;
            default:
                printf("Invalid choice\n");
            }
            break;
        case 4:
            printf("Goodbye!\n");
            return 0;
        default:
            printf("Invalid choice\n");
        }
    }
}
