# c-lab
this repository contains c lab programs
//Simple calculator program
#include<stdio.h>
int main()
{
  char op;
  int a,b,result;
  printf("\nEnter two operands : ");
  scanf("%d%d",&a,&b);
  printf("Choose operator : \n1.Addition\n2.Subtraction\n3.Multiplication\n4.Division\n5.Modulus\nEnter : ");
  scanf(" %c",&op);
  if(op=='+')
  {
    result=a+b;
  }
  else if(op=='-')
  {
    result=a-b;
  }
  else if(op=='*')
  {
    result=a*b;
  }
  else if(op=='/')
  {
    if(b==0)
    {
      printf("\nDivision not possible");
      return -1;
    }
    else
    {
      result=a/b;
    }
  }
  else if(op=='%')
  {
    if(b==0)
    {
      printf("\nDivision not possible");
      return -1;
    }
    else
    {
      result=a%b;
    }
  }
  else
  {
    printf("Invalid operator");
    return -1;
  }
  printf("%d %c %d = %d",a,op,b,result);
  return 0;
}
