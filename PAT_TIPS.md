最大公约数(辗转相除法)
```c++
#include <iostream>
using namespace std;
int gcd(int a, int b)
{
	if (b == 0) return a;
	else return gcd(b, a % b);
}//最大公约数
```

>对于任何素数a(1 < a < n), n % a != 0成立，也称为质数

>n % a == 0, 称为合数

>1既不是素数也不是合数

sqrt求给定数字的平方根