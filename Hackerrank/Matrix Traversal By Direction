#include <stdio.h>

int main()
{
   int i,j,N,M,temp,sr,sc;
   scanf("%d%d",&N,&M);
   printf("\n");
   int a[N][M],out[N*M];
   for(i=0;i<N;i++)
   {
       for(j=0;j<M;j++)
       {
           scanf("%d",&a[i][j]);
           printf("\n");
       }
   }printf("\n");
   char path[N*M];
   scanf("%d%d",&sr,&sc);
   printf("\n");
   scanf("%s",path);
   i=0,temp=0;
   do
   {
       out[i]=a[sr-1][sc-1];
       char command=path[i];

       switch(command)
       {
           case '>':    ++sc;    break;
           case '<':    --sc;    break;
           case '^':    --sr;    break;
           case 'v':    ++sr;    break;
       }


       if(sr>N || sc>M)
       {
           temp=1;
           printf("Invalid Input");
           break;
       }
       ++i;
   }while(path[i-1]!='\0');
   if(temp!=1)
   {
       printf("\n");
       for(j=0;j<i;j++)
       {
           printf("%d\t",out[j]);
       }
   }
   return 0;
}
