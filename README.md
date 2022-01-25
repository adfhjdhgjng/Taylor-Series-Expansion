//Taylor-Series-Expansion
#include<iostream.h>
#include<math.h>
int main ()
{
   float x,t,sum;
  int i,n=20;
  cout<<"Input X:\n";
  cin>>x;
  x=x*3.1412/180;
  t=t+1;
  sum=1;
  for(i=1; i<n; ++i)
{
   t=t*pow((double)(-1),(double)(2*i-1))*x*x/(2*i*(2*i-1));
   sum+=t;
}
cout<<"cos(x)="<<sum<<"\n";
return 0;
}
