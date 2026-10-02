#include <stdio.h>
int main()
{
    char binstr[100];
    unsigned int num =0;
    printf("Please enter a number in binary: ");
    scanf("%s", binstr);
    for(int i =0;binstr[i]!='\0';i++)
    {
        if(binstr[i]!='0'&& binstr[i]!='1')
       {
           printf("Invalid binary number\n");
           return 0; 
       }
       else
       {
        num = num*2 + (binstr[i]-'0');
       }
    }
    printf("the decimal equivalent of binary number %s is: %u\n", binstr, num);
    return 0;
}
