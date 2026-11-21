#include <stdio.h>
#include <string.h>

int main()
{
    char str1[200], str2[100], copy[200];
    int choice, result;

    printf("Enter first string: ");
    fgets(str1, sizeof(str1), stdin);
    str1[strcspn(str1, "\n")] = '\0';

    printf("Enter second string: ");
    fgets(str2, sizeof(str2), stdin);
    str2[strcspn(str2, "\n")] = '\0';

    do
    {
        printf("\n----- STRING OPERATIONS -----\n");
        printf("1. Find Length\n");
        printf("2. Copy String\n");
        printf("3. Join Strings\n");
        printf("4. Compare Strings\n");
        printf("5. Exit\n");

        printf("Enter your choice: ");
        scanf("%d", &choice);

        switch(choice)
        {
            case 1:
                printf("Length = %lu", strlen(str1));
                break;

            case 2:
                strcpy(copy, str1);
                printf("Copied String = %s", copy);
                break;

            case 3:
                strcat(str1, str2);
                printf("Joined String = %s", str1);
                break;

            case 4:
                result = strcmp(str1, str2);

                if(result == 0)
                    printf("Strings are equal");
                else
                    printf("Strings are not equal");
                break;

            case 5:
                printf("Exiting program");
                break;

            default:
                printf("Invalid choice");
        }

    } while(choice != 5);

    return 0;
}
