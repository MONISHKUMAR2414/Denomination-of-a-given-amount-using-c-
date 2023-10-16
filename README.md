# Denomination-of-a-given-amount-using-c-


#include <stdio.h>

int main()
{
    int amount,note;
    printf("Enter the amount= ");
    scanf("%d",&amount);
    
    int array[10]={500, 100, 50, 20, 10, 5,2,1};
    
    for(int i =0;i<sizeof(array);i++){
        note = amount/array[i];
        
        if(note){
            amount = amount%array[i];
            printf("%d*%d=%d\n",note,array[i],note*array[i]);
        }
    }
}
