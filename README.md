#include <stdio.h>

int main()
{
int t,n,i,k,s;
int a[1000];
int min;
scanf("%d ",&t);
if(t<6)
{ while(t)
{
s=0;
scanf("%d %d",&n,&k);
for(i=0;i<n;i++)
{
scanf("%d ",&a[i]);
}
min=a[0];
for(i=1;i<n;i++)
{
if(a[i]<min)
{
min=a[i];
}
}
if(k>=min)
s=k-min;
else
s=0;

printf("%d\n",s);
t--;
}
}

}
