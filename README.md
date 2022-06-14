# Renaissance
![image](https://user-images.githubusercontent.com/105922890/173496341-79e8b44c-6b39-4f9a-9447-ac6417e95e49.png)
#include <stdio.h>
#include <math.h>
int main()
{
	double x1 = 1.5, x0 = 0, f, f1;
	while (fabs(x1 - x0) >= 1e-6)
	{
		x0 = x1;
		f = ((2 * x0 - 4) * x0 + 3) * x0 - 6;
		f1 = (6 * x0 - 8) * x0 + 3;
		x1 = x0 - f / f1;
	}
	printf("方程在1.5附近的根为:%lf\n", x1);
	return 0；
}
