#include <stdio.h>
#include <string.h>
int main(int argc, char *argv[]) {
    if (argc != 3) {
        printf("Usage: %s [Operating System] [SSE]\n", argv[0]);
        return 1;
    }
    char *search_string = argv[1];
    char *file_name = argv[2];
    FILE *file = fopen(file_name, "r");
    if (!file) {
        printf("Error opening file\n");
        return 1;
    }
    char line[256];
    while (fgets(line, sizeof(line), file)) {
        if (strstr(line, search_string)) {
            printf("%s", line);
        }
    }
    fclose(file);
    return 0;
}
