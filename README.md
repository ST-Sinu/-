level 0

#include <stdio.h> // 컴파일러에서 제공해주는 헤더파일 printf, scanf_s 등등 있음
                   // "head.h"등을 이용하면 미리 정해주지 않은 헤더파일 
                       만들어서 사용한 것

int main(void) // main이 정수형 데이터를 반환 할 수 있음을 나타냄
               // void main은 main이 어떤 값도 반환하지 않음
{
  int num1 = 100, num2 = 100; // int형 전수 num1과 num2를 각각 선언한다.
  int * pnum; // int형 포인터 변수 pnum을 선언한다.
              
  
  pnum = &num1; // 포인터 pnum이 num1을 가리킴
  (*pnum) += 30; // [*pnum = num] num1 += 30; 과 동일하다
  
  pnum = &num2; // 포인터 pnum이 num2를 가리킴
  (*pnum) -= 30; // num2 -= 30; 과 동일하다
  
  printf("num1 : %d, num2 : %d \n", num1, num2);
  return 0;
}
