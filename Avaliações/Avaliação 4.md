Implemente um programa na linguagem C que faça as seguintes
funcionalidades:
1) Dada uma Matriz Quadrada m
que é passada para uma função soma_linha( m, slinha, n)
onde slinha é um array e
n é o tamanho da matriz quadrada.
Calcular a soma dos elementos de cada linha da matriz m(i,j)
e armazenar a soma no array slinha (i).
*/
#include <stdio.h>
#define TAMANHO 4
int exibe_vetor(int tamanho, int vetor[tamanho])
{
int i;
for(i = 0; i < tamanho; i++)
{
printf("%2d ", vetor[i]);
}
printf("\n");
}
int exibe_matriz(int tamanho, int matriz[tamanho][tamanho])
{
int i, j;
for(i = 0; i < tamanho; i++)
{
for(j = 0; j < tamanho; j++)
{
printf("%2d ", matriz[i][j]);
}
printf("\n");
}
}
void soma_linha(int tamanho, int matriz[tamanho][tamanho], int
vetor_soma[tamanho])
{
int i, j;
for ( i = 0; i < tamanho; i++)
{
vetor_soma[i] = 0;
for ( j = 0; j < tamanho; j++)
{
vetor_soma[i] += matriz[i][j];
}
}
}

int main()
{
int m[TAMANHO][TAMANHO] = {

{27, 27, 27, 27},

{28, 28, 28, 28},
{29, 29, 29, 29},
{21, 21, 21, 21}
};

int slinha[TAMANHO];
soma_linha (TAMANHO, m, slinha);
exibe_matriz(TAMANHO, m);
exibe_vetor (TAMANHO, slinha);
return 0;
}
