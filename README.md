# c-using-to-count-no-of-alphabets
#include<stdio.h>
#define MAX_SIZE 100
int main(){
  char str[MAX_SIZE];
  int alphabets,digits,others,i;
  alphabets=digits=others=i=0;
  printf("enter sny string:");
  scanf("%s",str);
  while(str[i]!='\0'){
    if((str[i]>='a' && str[i]<='z')||(str[i]>='A' && str[i]<='Z')){
      alphabets++;
    }
    else if(str[i]>='0' && str[i]<='9'){
      digits++;
    }
    else{
      others++;
    }
    i++;
  }
  printf("alphabets=%d\n",alphabets);
  printf("digits=%d\n",digits);
  printf("special characters=%d\n",others);
  return 0;
}
