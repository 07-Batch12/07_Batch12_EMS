#include<stdio.h>
#include<conio.h>
#include<string.h>
void bill();
void details();
struct ems
{
	int id_num,mtr_num,ch;
	char name[20],st_name,a_name[20],dis_name[20],h_name[8];
	float puc,cons_unit,bill,c_read,uc_read;
}e;
void main()
{
	clrscr();
	printf("\n Enter Your Full Name :  ");
	gets(e.name);
	printf("\n Enter Id Number :  ");
	scanf("%d",&e.id_num);
	printf("\n Enter Meter Number : ");
	scanf("%d",&e.mtr_num);
	printf("\n Enter House Number : ");
	scanf("%s",&e.h_name);
	printf("\n Enter Area Name : ");
	scanf("%s",&e.a_name);
	printf("\n Enter District : ");
	scanf("%s",&e.dis_name);
	printf("\n Your consumption in kilowatt : ");
	scanf("%f",&e.cons_unit);
	printf("\n Per unit charge : ");
	scanf("%f",&e.puc);
	printf("\n Current Reading : ");
	scanf("%f",&e.c_read);
	printf("\n REQUEST FOR CHANGE IN LAST READING (PRESS 1 FOR yes/2 FOR no)");
	scanf("%d",&e.ch);
	if(e.ch==1)
	{
		printf("Enter Updated Reading : ");
		scanf("%f",&e.uc_read);
		e.c_read=e.uc_read;
		printf("\n Current Reading : %f",e.c_read);
		getch();
		details();
		bill();
		printf("\n Bill : %f",e.bill);
	}
	else if (e.ch==2)
	{
		details();
		bill();
		printf("\n Bill : %f",e.bill);
	}
	else
	{
		printf("\n Invalid Input");
	}
	getch();
}
void bill()
{
	if(e.cons_unit>1 && e.cons_unit<=2)
	{
		e.bill=500+(e.cons_unit-1)*1000*e.puc;
	}
	else if(e.cons_unit<1)
	{
		e.bill=(e.cons_unit*1000)*e.puc;
	}
	else if(e.cons_unit>2 && e.cons_unit<=5)
	{
		e.bill=900+(e.cons_unit-1)*1000*e.puc;
	}
	if(e.cons_unit>5 && e.cons_unit<=10)
	{
		e.bill=1500+(e.cons_unit-1)*1000*e.puc;
	}
	if(e.cons_unit>10)
	{
		e.bill=900+(e.cons_unit-1)*1000*e.puc;
	}
	getch();
}
void details()
{
	clrscr();
	printf("\n Enter Your Full Name : %s",e.name);
	printf("\n Enter Id Number : %d ",e.id_num);
	printf("\n Enter Meter Number : %d ",e.mtr_num);
	printf("\n Enter House Number : %s ",e.h_name);
	printf("\n Enter Area Name : %s",e.a_name);
	printf("\n Enter District : %s",e.dis_name);
	printf("\n Your consumption in kilowatt : %f",e.cons_unit);
	printf("\n Per unit charge : %f",e.puc);
	printf("\n Current Reading : %f",e.c_read);

	getch();
}
