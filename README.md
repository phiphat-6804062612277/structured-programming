#include <stdio.h>
int main(){
	int mid,final,q1,q2,lab,sit;
//	mid = 75 ; final = 85; q1 = 40;
//	q2 = 45 ; lab = 16; sit=15;	
	//input
	scanf("%d %d %d %d %d %d",&mid,&final,&q1,&q2,&lab,&sit);
	//Operator
	float a1 = ((float)mid/100)*30;
	float a2 = ((float)final/120)*35;
	float a3 = ((float)q1/60)*12;
	float a4 = ((float)q2/60)*13;
	float a5 = ((float)lab/16)*5;
	float a6 = ((float)sit/16)*5;
	float sum = ((float)a1+(float)a2+(float)a3+(float)a4+(float)a5+(float)a6);
	printf("%10s=%8d => %f\n","Mid",mid,a1);
	printf("%10s=%8d => %f\n","Final",final,a2);
	printf("%10s=%8d => %f\n","Q1",q1,a3);
	printf("%10s=%8d => %f\n","Q2",q2,a4);
	printf("%10s=%8d => %f\n","Lab",lab,a5);
	printf("%10s=%8d => %f\n","Sit",sit,a6);
	printf("*****%f*****",sum);
//	printf("%10s=%8d \n","Mid",mid);
//	printf("%10s=%8d \n","Final",final);
//	printf("%10s=%8d \n","Q1",q1);
//	printf("%10s=%8d \n","Q2",q2);
//	printf("%10s=%8d \n","Lab",lab);
//	printf("%10s=%8d \n","Sit",sit);
}
