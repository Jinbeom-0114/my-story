// line2를 line1에 붙이기
#include <stdio.h>
int main(void)
{
	char line1[81], line2[81];
	int i=0, k=0;

	printf("쳐");
	gets_s(line1, 81);

	printf("쳐");
	gets_s(line2, 81);

	while (line1[i] != '\0') {
		i++;
	}
	while (line2[k] != '\0') {
		line1[i] = line2[k];
		i++;
		k++;
	}
	line1[i] = '\0';
	printf("result:%s", line1);
	return 0;
}
