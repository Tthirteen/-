
#include<stdio.h>
int main()
{
	int a,b,c,d,m,n=0;
	int sum=0;
	int i=1;
	for(i=1;i<=9;i++)
	{
		for(m=i*1000;m<=i*1000+999;m++)
		{
			d=m%10;
	        c=(m/10)%10;
	     	b=(m/100)%10;
	    	a=m/1000;
	    if(a+b==c+d)
			n++;
		}
		printf("%d000~%d999之间有%d个满足要求的数\n",i,i,n);
		sum+=n;
	}
	printf("1000~9999之间一共有%d个满足要求的数\n",sum);
	return 0;
}


  



 
