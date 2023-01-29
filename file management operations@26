#include <stdio.h>
#include <stdlib.h>
int main()
{
char character;
FILE *fpointer;
fpointer = fopen("C:\\program.txt","w"); 
if(fpointer == NULL)
{
printf("Error! The file does not exist.");
exit(0);
}
printf("Enter a character: ");
scanf("%c",&character);
fprintf(fpointer,"%c",character); 
fclose(fpointer);
return 0;
}
