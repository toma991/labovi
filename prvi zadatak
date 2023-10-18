#include <stdio.h>
#include <stdlib.h>
#define MAX_LENGTH 50

typedef struct _student {
    char ime[MAX_LENGTH];
    char prezime[MAX_LENGTH];
    int bodovi;
} student;

int main() {
    int i = 0, count = 0;
    char ch;
    FILE* data;
    data = fopen("studenti.txt", "r");
    if (data == NULL) {
        printf("Error: Unable to open the file.\n");
        return 1; 
    }

    while ((ch = fgetc(data)) != EOF) {  
        if (ch == '\n')
            count++;
    }

    fclose(data);
    printf("Number of lines in the file: %d\n", count);
    return 0;
}
}
