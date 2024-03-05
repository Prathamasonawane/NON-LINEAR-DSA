/*Write a C program for the implementation of Topological sorting.*/

#include<stdio.h>
#include<stdlib.h>
#define max 50
struct stack
{
	int data[max];
	int top;
};
struct stack s;
int i,j,n,a[10][10];
void init()
{
	s.top=-1;
}
int isfull()
{
	return(s.top==max-1);
}
int isempty()
{
	return(s.top=-1);
}
void  push(int v)
{
	s.data[++s.top]=v;
}
int pop()
{
	return(s.data[s.top--]);
}
void Topological()
{
	int v[10]={0};
	init();
	int ind[10]={0};
	 for(i=1;i<=n;i++)
	  {
	   for(j=1;j<=n;j++)
	    {
	    ind[i]=ind[i]+a[j][i];
	    }
	   }
	   while(1)
	   {
	    for(i=1;i<=n;i++)
	     {
	      if(ind[i]=0 && v[i]==0)
	      push(i);
	      printf("v%d\t",i);
	     }
	     if(isempty())
	     break;
	     int v=pop();
	     for(j=1;j<=n;j++)
	      {
	        if(a[v][j]==1)
	        ind[j]=ind[j]-1;
	      }
	   }
}
int main()
{
	printf("Enter Number of Vertice:");
	scanf("%d",&n);
	printf("Enter Matrix:");
	 for(i=1;i<=n;i++)
	   {
	     for(j=1;j<=n;j++)
	       { 
	         scanf("%d",&a[i][j]);
	       }
	    }
	    Topological();
}
	      
	
