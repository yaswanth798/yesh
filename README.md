#include <stdio.h>
int main()
{
  int amount=5000;
  printf("Enter 1:Account Balance:\nEnter 2:cash with drawl:\nEnter 3:Cash Deeposit:\n");
  while(1)
  {
    printf("Enter your choice (1 to 3):\n");
    int ch,rs;
    scanf("%d",&ch);
    if(ch==1)
    {
      printf("Account Balance:%d\n",amount);
    }
    else if(ch==2)
    {
      printf("Enter the amount to withdraw:");
      scanf("%d",&rs);
      if(rs>amount)
      {
        printf("Insufficient Balance\n");
    }
    else
    {
      amount=amount-rs;
      printf("Account Balance:%d\n",amount);
    }
    }
    else if(ch==3)
    {
    printf("Enter the amount to Deeposit:");
    scanf("%d",&rs);
    amount=amount+rs;
    printf("Account Balance:%d\n",amount);
    }
    else
    {
      printf("Do you want to continue (type y for continue):\n");
      char d;
      scanf("%c",&d);
      if(d!='y')
      {
      printf("Thank you!\n");
  break;
      }
    }
    return 0;
}
}
  
