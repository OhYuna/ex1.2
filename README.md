#include <stdio.h>

int main(void)
{
	float a;
	float b = 1.0;
	float sum = 0;
	int m = 2;


	for (a = 2.0; a <= 100.0; a++)
	{
		if (a == 100)
			printf("%.0lf/%.0lf ", b, a);
		else
			printf("%.0lf/%.0lf + ", b, a);
		if (m % 10 == 0)
			printf("\n");
		sum += b / a;		
		b++;
		m++;
	}

	printf(" = %lf \n", sum);
	return 0; 
}
