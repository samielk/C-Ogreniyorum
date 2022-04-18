# C-Ogreniyorum

#include <stdio.h>

#include <stdlib.h>

int main()
{
    printf("Matrikslerle carpma islemi \n");
    
    printf("\n-------------------------------------------------------------------------------\n\n");
    
    int m,n,i,j,k,carp,say,a[100][100],b[100][100],c[100][100];

    printf("Matriks kac satir olsun? : ");scanf("%d",&m);
    printf("Matriks kac sutun olsun? : ");scanf("%d",&n);

    printf("\n---------------- A  dizisi degerlerini girin ---------------\n\n");


    for(i=1;i<=m;i=i+1)
        {
                   for(j=1;j<=n;j++)
                {
                    printf("[A] Dizisinin %d. satirin %d. Sutunu degerlerini girin.:  ",i+0,j+0);
                    scanf("%d",&a[i][j]);
                }


        }

  printf("\n---------------- B  dizisi degerlerini girin ---------------\n\n");
    for(i=1;i<=m;i++)
        {

                for(j=1;j<=n;j++)
                {
                    printf("[B] Dizisinin %d. satirinin %d Sutun degerlerini girin. :  ",i+0,j+0);
                    scanf("%d",&b[i][j]);
                }

        }

printf("\n-------------------Hesaplanan C dizisi ---------------\n\n");


    for(i=1;i<=m;i=i+1)
        {
           say=0;

            for(j=1;j<=n;j++)
            {
                carp=1;
                for(k=1;k<=2;k++)

                    carp=carp=a[i][k]*b[k][j];
                    c[i][j]=carp;
                    printf("                  %d      ",c[i][j]);
                    say=say+1;


            if (say==2)printf("\n");
            }
  printf("\n-----------------------------------------------------------\n\n");

        }






    return 0;
}




[Matriks carpma siralamasi-v01.xlsx](https://github.com/samielk/C-Ogreniyorum/files/8504483/Matriks.carpma.siralamasi-v01.xlsx)
