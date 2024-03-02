/*Write a C program that accepts the vertices and edges of a graph and store it as an
adjacencymatrix. Implement function to traverse the graph using Breadth First Search (BFS)
traversal.*/


#include<stdio.h>
#define MAX 30
struct que
{
	int data[MAX];
	int front,rear;
	}q;
	void initq()
	{
	q.front=q.rear=-1;
	}
	int isempty()
	{
	return(q.front==q.rear);
	}
	void addq(int num)
	{
	q.rear++;
	q.data[q.rear]=num;
	}
	int delq()
	{
	int num;
	q.front++;
	num=q.data[q.front];
	return(num);
	}
	void bfs(int a[10][10],int n)
	{
	int visited[10]={0};
	int i,j;
	initq();
	i=1;
	visited[i]=1;
	addq(i);
	while(!isempty())
	{
	i=delq();
	printf("%d\t",i);
	for(j=1;j<=n;j++)
	{
	if(a[i][j]==1 && visited[j]==0)
	{
	addq(j);
	visited[j]=1;
	}
}
}
}
	int main()
	{
	int a[10][10],n,i,j;
	printf("\n enter limit:");
	scanf("%d",&n);
	printf("\n the adjacency matrix\n");
	for(i=1;i<=n;i++)
	{
	for(j=1;j<=n;j++)
	{
	scanf("%d",&a[i][j]);
	}
}
	printf("\n BFS traversal :");
	bfs(a,n);
	}
