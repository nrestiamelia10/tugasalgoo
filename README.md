#include <iostream>
#include<stdio.h>
#include<stdlib.h>
using namespace std;
float desimal(float a, float b)
{
    float c;
    c=a/b;
    return c;
}
int bulatkan (float bulat)
{
     int a,c;
     float d;
     a=bulat;
     d=(bulat-a);
     if(d>=0.5)
     {
         return a+1;
     }
     else {return a;}

}
int main (void)
{
    int a,b,hasil;
    float bulat;
    printf("Masukkan pembilang :");
    scanf("%d",&a);
    printf("Masukkan penyebut  :");
    scanf("%d",&b);
    printf( "           %d",a);
    printf("\n");
    printf("Pecahan :  -");
    printf("\n");
    printf("           %d",b);
    printf("\n");
    bulat=desimal(a,b);
    printf("Hasil konversi ke desimal  :");
    printf("%d\n",bulat);
    hasil=bulatkan(bulat);
    printf("Setelah dibulatkan         :");
    printf("%d\n",hasil);
    system("pause");
    return 0;
}
