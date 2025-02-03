#include <stdio.h>
#include<ctype.h>
int main()
{
  char c;
  scanf("%c",&c);
  c=tolower(c);
  if("c=='a' || c=='e' || c=='i' || c=='o' || c=='u'")
  {
  printf("vowel");
}
else if(isalpha(c))
{
  printf("consonents");
}
else
{
  printf("not a alphabet");
}
return 0;
}
