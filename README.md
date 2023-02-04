//# binary_ip_address.c//
#include<stdio.h>
#include<string.h>
int main()
{
    int i,s[32];
    printf("Enter IP address in binary form:");
     for(i=0;i<32;i++)
     {  
        scanf("%d",&s[i]);
        if(s[i]==0|| s[i]==1)
        {
        }
        else
        {
            printf("it is a invalid IP address\n");
        }
     }
      printf("binary ip address is:");
     for(i=0;i<32;i++)
     {
        printf("%d",s[i]);
     }
     if(s[0]==0)
     {
        printf("\nThis IP address belongs to Class A");
     }
     else if(s[0]==1 && s[1]==0)
     {
        printf("\nThis IP address belongs to class B");
     }
     else if(s[0]==1 && s[1]==1 && s[2]==0)
     {
        printf("\n This IP address belongs to class C");
     }
     else if(s[0]==1 && s[1]==1 && s[2]==1 && s[3]==0)
     {
        printf("\n This IP address belongs to class D");
     }
     else
     {
        printf("\nThis IP address belongs to Clsss E");
     }
}
