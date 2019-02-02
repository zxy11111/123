#include<stdio.h>
#include<math.h>
struct a
{
	int t;
	bool p;
}e[10000];
int c[10000];
void main()
{
	int n,i,k,j,l=0,p,m,q=0;
	while(scanf("%d",&n)!=EOF&&n>=2&&n<=10000)
	{
		for(i=0;i<n;i++)
		{
			e[i].t=i+1;
			e[i].p=true;
			for(k=2;k<=sqrt(i+1)+1;k++)
			{
				if((i+1)%k!=0)
				{
					c[l++]=k;
				}
			}
			for(p=0;p<l;p++)
			{
				for(m=2;m*c[p]<=n;m++)
				{
					e[(m*c[p])-1].p=false;
				}
			}
			l=0;
		}
		e[0].p=false;
		for(i=0;i<n;i++)
		{
			if(e[i].t%10==1&&e[i].p==true)
			{
				printf("%d ",e[i].t);
				q=1;
			}
		}
		if(q==0) printf("%d",q-1);
	}
}
