# Variable
---

변수란 변경될 가능성이 있는 수를 의미한다.   

변경될 가능성이 있는 수를 표현하기 위해 어떠한 방법을 사용하고 있는지 알아보자.   
1. 변수의 선언을 통해 메모리 공간을 확보한다.
2. 확보한 메모리 공간에 특정한 값을 저장한다.
3. 식별자를 통해 메모리 공간에 저장된 값을 표현한다.
4. 언제든지 확보한 메모리 공간에 재접근하여 값을 변경할 수 있다.

int example; --- (1) 변수 선언, 메모리 공간 확보   
example = 20; --- (2) 확보한 메모리 공간에 특정한 값을 저장   
std::cout << example << std::endl; --- (3) 변수의 식별자를 통해 값을 표현   
example = 50; --- (4) 확보된 메모리 공간에 재접근하여 값을 변경   

변수의 자료형은 메모리 공간의 크기와 CPU가 어떻게 해석하도록 할 것인지를 결정하고   
변수의 식별자는 CPU가 메모리 공간에 접근할 때 사용되는 주소의 별칭이라 할 수 있다.

일반적인 경우 변수의 식별자를 통해 메모리 공간에 저장된 값을 표현하며   
L-value로 사용되는 경우에는 메모리 공간 자체를 의미한다.

1. 대입 연산자를 기준으로 왼쪽을 L-Value, 오른쪽을 R-Value로 생각하면 쉽다.
int a = 10; (L-value = R-value)   

2. 포인터 변수는 변수의 주소를 저장하는 용도로 사용된다.
int* ptr = &a;   
->lea rax, [rbp-12]   
->mov QWORD PTR [rbp-8], rax   

3. 접근에 한해서는 식별자 == *(&식별자)라 할 수 있다.
*ptr == *(&a) == a
