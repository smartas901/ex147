ex1471.h
#ifndef EX1471_H
#define EX1471_H
double sumofvector(double *a, size_t);
#endif
ex1471.c
#include<ex1471.h>
#include<stdio.h>
double sumofvector(double *a, size_t len)
{
        int i;
        double sum = 0;

        for(i = 0;i < len;i++)
                sum = sum + a[i];

        return sum;
}
ex1472.h
#ifndef EX1472_H
#define ex1472_H
double sumofvectorp(double *a, size_t len);
#endif
ex1472.c
#include<ex1472.h>
#include<stdio.h>
double sumofvectorp(double *a, size_t len)
{
        int i;
        double sum = 0;

        while(len--)
                sum = sum *a++;

        return sum;
}
ex1473.c
#include<ex1471.h>
#include<ex1472.h>
#include<stdio.h>
int main(void)
{
        int a[5];
        int counter = 0;
        size_t len = 5;

        while(counter < 5)
                a[counter] = counter + 0.5;
        printf("The sum of a is: %lf \n".sumofvector(&a,len);;
        return 0;;
}
