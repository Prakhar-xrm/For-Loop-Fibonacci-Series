#include <stdio.h>
int main(){
  
  int num;
  int i;
  int a = 0, b = 1;
  int next;
  
  scanf("%d", &num);
  
  printf("Fibonacci Series: ");
  
  for(i = 0; i < num; i++){
    if(i <= 1){
      next = i;
    }
    else{
      next = a + b;
      a = b; b = next;
    }
    printf("%d ", next);
  }
  return 0;
}
