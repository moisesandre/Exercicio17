# Exercicio17

#include <stdlib.h>
#include <stdio.h>
main ()
{
    system("color 0b");
    int idade[20], i;
    float peso[20], m1=0,m2=0,m3=0,m4=0;

    for (i=0; i<=19; i++)
    {
        printf("\nDigite sua idade: ");
        scanf("%d",&idade[i]);
        printf("\nDigite seu peso:");
        scanf("%f",&peso[i]);
    }

    for (i=0; i<=19; i++)
    {
        if(idade[i]<=10)
        {
            m1=m1+peso[i];
        }
        if(idade[i]>=11 && idade[i]<=20)
        {
            m2=m2+peso[i];
        }
        if(idade[i]>=21 && idade[i]<=30)
        {
            m3=m3+peso[i];
        }
        if (idade[i]>30)
        {
            m4=m4+peso[i];
        }
    }

    printf("a media de peso entre 1 a 10 anos e %.2f\n", m1/2);
    printf("a media de peso entre 11 a 20 anos e %.2f\n", m2/2);
    printf("a media de peso entre 21 a 30 anos e %.2f\n", m3/2);
    printf("a media de peso acima de 30 anos e %.2f", m4/2);

    return 0;
}
