* Variable

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
