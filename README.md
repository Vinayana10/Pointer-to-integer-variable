# Pointer-to-integer-variable

#include<stdio.h>
#include<stdlib.h>
int main() {
    
    int *x;//static memory
    x=(int*)malloc(sizeof(int));//dynamic memory
    printf("x=%p",x);
    if(x==NULL)
    {
      perror("allocation failed!");  
    }
    *x=10;
    printf("value of x=%d \n",*x);
    char *name=(char *)malloc(50*sizeof(char));
    name="VIIT";
    printf("%s",name);
    return 0;
}
