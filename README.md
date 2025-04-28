#include <stdio.h>
#include <stdlib.h>
void generate_invisible_text(int length) {
    for (int i = 0; i < length; i++) {
        putchar(' ');
    }
    putchar('\n');
}
int main() {
    int length;

    printf("Welcome to the Invisible Text Generator!\n");
    printf("How long do you want your invisible text to be? (number): ");
    
    if (scanf("%d", &length) != 1 || length < 0) {
        printf("Error: Please enter a valid positive number!\n");
        return 1;
    }

    printf("\nHere is your invisible text:\n\n");
    generate_invisible_text(length);

    printf("\nYou're welcome. Stay invisible!\n");
    return 0;
}
