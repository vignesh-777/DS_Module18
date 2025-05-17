# Ex 5(d) Travelling Salesman Problem
## DATE:12/05/2025
## AIM:
To write a C Program to implement Travelling Salesman Problem for finding shortest path.
## Algorithm
1. Start
2. Read the number of cities n and the adjacency matrix a representing the distances between 
cities.
3. Initialize a visited array to track which cities have been visited.
4. Start the process with city 0 and print its number.
5. In the mincost function, find the nearest unvisited city using the least function.
6. If all cities are visited, return to the starting city (city 0) and finish.
7. In the least function, find the unvisited city with the smallest cost from the current city, and update the cost.
8. Print the minimum cost of the route after visiting all cities.
9. End

## Program:
```
/*
Program to implement Travelling Salesman Problem for finding shortest path
Developed  By: VIGNESH R
Reg No :212223240177
*/
#include<stdio.h>
int a[10][10],visited[10],n,cost=0;
voidget()
{
int i,j;
scanf("%d",&n);
for(i=0;i<n;i++)
{
for( j=0;j < n;j++) 
scanf("%d",&a[i][j]);
visited[i]=0;
}
}
void mincost(int city)
{
int ncity;
int least(int); 
visited[city]=1; 
printf("%d-->",city+1); 
ncity=least(city);
update the cost.
8. Print the minimum cost of the route after visiting all cities.
9. End
if(ncity==999)
{
ncity=0; 
printf("%d",ncity+1); 
cost+=a[city][ncity]; 
return;
}
mincost(ncity);
}
int least(int c)
{
int i,nc=999;
int min=999,kmin; 
for(i=0;i< n;i++)
{
if((a[c][i]!=0)&&(visited[i]==0)) 
if(a[c][i] < min)
{
}
}
}
if(min!=999)
cost+=kmin; 
return nc;
min=a[i][0]+a[c][i]; 
kmin=a[c][i];
nc=i;
voidput()
{
printf("\n\nMinimum cost:%d",cost);
}
int main()
{
get(); 
mincost(0); 
put(); 
return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/84fbb7a3-a470-4169-9560-4477bd996e47)



## Result:
Thus, the C program to implement Travelling Salesman Problem for finding shortest path is implemented successfully.
