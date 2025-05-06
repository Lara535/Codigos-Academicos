# Codigos-Academicos
---
### ⭐ Exemplos de alguns dos códigos feitos durante estudos da linguagem em C: 

#include <stdio.h>

int main(){
    float a, b, c, perimetro, area;

    scanf("%f %f %f", &a, &b, &c);
    
    perimetro = a + b + c;
    area = ((a+b)*c)/2;

    if(a + b > c && a + c > b && b + c > a)
       printf("Perimetro = %.f\n", perimetro);

    else
       printf("Area = %.f\n", area);

    return 0;
}
---

#include <stdio.h>

int main(){
    float valor, total, x, reaju;
    int p15, p12, p10, p7, p4;

    scanf("%f", &valor);

    x = p15 || p12 || p10 || p7 || p4
    p15 = 15;
    p12 = 12;
    p10 = 10;
    p7 = 7;
    p4 = 4;

    total = valor + (valor * x/100);
    reaju = total - valor;

    if(valor>= 0 && valor <= 400){
        x = p15;
        total = valor + (valor * x/100);
        reaju = total - valor;
        printf("Novo salario: %.2f\n", total);
        printf("Reajuste ganho: %.2f\n", reaju);
        printf("Em percentual: 15 "%"\n");
    }

    else if(valor>= 400.01 && valor <= 800){
         x = p12;
         total = valor + (valor * x/100);
         reaju = total - valor;
         printf("Novo salario: %.2f\n", total);
         printf("Reajuste ganho: %.2f\n", reaju);
         printf("Em percentual: 12 %\n");
         }


    else if(valor>= 800.01 && valor <= 1200){
             x = p10;
             total = valor + (valor * x/100);
             reaju = total - valor;
             printf("Novo salario: %.2f\n", total);
             printf("Reajuste ganho: %.2f\n", reaju);
             printf("Em percentual: 10 %\n");
             } 

    else if(valor>= 1200.01 && valor <= 2000){
                 x = p7;
                 total = valor + (valor * x/100);
                 reaju = total - valor;
                 printf("Novo salario: %.2f\n", total);
                 printf("Reajuste ganho: %.2f\n", reaju);
                 printf("Em percentual: 7 %\n");
                 }

    else if(valor > 2000){
                     x = p4;
                     total = valor + (valor * x/100);
                     reaju = total - valor;
                     printf("Novo salario: %.2f\n", total);
                     printf("Reajuste ganho: %.2f\n", reaju);
                     printf("Em percentual: 4 %\n");
                     }

    return 0;
}
---

#include <stdio.h>

int main()
{
    double n1, n2, n3, n4, media;
    double  nE, medExame;

    scanf("%lf %lf %lf %lf", &n1, &n2, &n3, &n4);

    media = (n1*2 + n2*3 + n3*4 + n4*1)/10;
    
    printf("Media: %lf\n", media);

    if(media>= 7)
       printf("Aluno aprovado.\n");
    else 
        if(media < 5)
            printf("Aluno reprovado.\n");
        else
            if(media >= 5 && media <= 6.9)
            {
                printf("Aluno em exame.\n");
                scanf("%lf", &nE);
                printf("Nota do exame: %lf\n", nE);
                medExame = (nE + (n1*2 + n2*3 + n3*4 + n4*1)/10)/2;
                if (medExame >= 5)
                    printf("Aluno aprovado.\n");
                else
                    printf("Aluno reprovado.\n");
                printf("Media final: %lf\n", medExame);
            }
    return 0;
}
---

#include <stdio.h>

int main() {
    float valor;
    int n100, n50, n20, n10, n5, n2;
    int m1, m05, m025, m010, m005, m001; 

    scanf("%.2f", &valor);

    n100 = valor/100;
    n50 = (valor - n100 * 100)/50;
    n20 = ((valor - n100 * 100) -n50 * 50)/20;
    n10 = (((valor - n100 * 100) -n50 * 50) -n20 * 20)/10;
    n5 = ((((valor - n100 * 100) -n50 * 50) -n20 * 20) -n10 * 10)/5,
    n2 = (((((valor - n100 * 100) -n50 * 50)- n20 * 20) -n10 * 10)- n5 * 5)/2;

    m1 = valor/1;
    m05 = (valor - m1 * 1)/0.5;
    m025 = ((valor - m1 * 1)-m05 * 0.5)/0.25;
    m010 = (((valor - m1 * 1) -m05 * 0.5) -m025 * 0.25)/0.10;
    m005 = ((((valor - m1 * 1) -m05 * 0.5) -m025 * 0.25) -m010 * 0.10)/0.05;
    m001 = (((((valor - m1 * 1) -m05 * 0.5) -m025 * 0.25) -m010 * 0.10) -m005 * 0.05)/0.01;


    printf("NOTAS: \n");
    printf("%d nota (s) de R$ 100,00\n", n100);
    printf("%d nota (s) de R$ 50,00\n", n50);
    printf("%d nota (s) de R$ 20,00\n", n20);
    printf("%d nota (s) de R$ 10,00\n", n10);
    printf("%d nota (s) de R$ 5,00\n", n5);
    printf("%d nota (s) de R$ 2,00\n", n2);
    printf("MOEDAS: \n");
    printf("%d moeda (s) de R$ 1,00\n", m1);
    printf("%d moeda (s) de R$ 0,50\n", m05);
    printf("%d moeda (s) de R$ 0,25\n", m025);
    printf("%d moeda (s) de R$ 0,10\n", m010);
    printf("%d moeda (s) de R$ 0,05\n", m005);
    printf("%d moeda (s) de R$ 0,01\n", m001);

    return 0;
}
---

#include <stdio.h>

int main(){
    int horaI, minI, horaF, minF, hTot, mTotal;

    scanf("%d %d %d %d", &horaI, &minI,&horaF, &minF);

    hTot = horaF - horaI;
    mTotal = minF - minI;

    if(hTot == 0){
        printf("O jogo durou 24 hora(s) e %d minuto(s).\n", mTotal);
    }    

        else if (hTot != 0 && mTotal != 0){
         printf("O jogo durou %d hora(s) e %d minuto(s). "\n, hTot, mTotal);
        }
    return 0;
}
---

#include <stdio.h>

int main (){
    int A, B, C, ari, pond;
    char opcao;

    scanf("%d %d %d", &A, &B, &C);
    printf("Escolha o formato da sua media:\n a- aritmetica\n p- ponderada\n");
    scanf("%c", &opcao);

    if(opcao == 'a'){
        ari = A + B + C/ 3;
        printf("a: %d\n", ari);
    }
    else if(opcao == 'p'){
            pond = (A * 3)+(B * 3)+(C * 4)/ A + B + C;
            printf("p: %d\n", pond);

    }
    return 0;
}
---

#include <stdio.h>
#include <stdlib.h>

int main() {
    
    char nome[50];
    float totalvendas, salariofixo;
    
    printf("***Program iniciado***\n");
    printf("Entre com nome, salario fixo, e total vendas\n");
    scanf("%s%f%f", &nome, &salariofixo, &totalvendas);
    printf("NOME = %s\n", nome);
    printf("TOTAL = R$ %.2f\n", 
        ((0.15 * totalvendas) + salariofixo));
    printf("***Programa finalizado***\n");
 
    return 0;
}

