a) Dados de entrada (a, b, c inteiros que correspondem na função quadrática F(x) =
ax**2 + bx + c). Pede-se as raizes da função quando Delta = 0 e Delta > 0. Quando
o Delta for < 0 printar a mensagem "Raízes Imaginárias"


#include <stdio.h>
#include <math.h>

int main()
{
    int a, b, c;
    int delta;
    float  x1, x2;
   
    printf("informe tres numeros inteiros: ");
    scanf ("%d %d %d", &a, &b, &c);
   
    delta = b*b - 4*a*c;
   
    printf ("delta = %d\n", delta);
   
    if ( delta < 0 )
    {
        printf ("raizes imaginarias\n");
    } else {
        x1 = (-b - sqrt(delta))/(2*a);
        x2 = (-b + sqrt( delta))/(2*a);
       
        printf ("primeira raiz da função %f\nsegunda raiz da função %f\n ", x1, x2);
    }

    return 0;
}

b) Dada uma String qualquer inverter essa String.

#include <stdio.h>
#include <string.h>
#include <locale.h>
  
void inverte(char *texto)
{
    setlocale(LC_ALL, "Portuguese");
    int posicao, comprimento, auxiliar;
    comprimento = strlen(texto);
    
    for (posicao = 0; posicao < comprimento/2; posicao++)
    {
        auxiliar = texto[posicao]; // texto[0] = 'G';
        texto[posicao] = texto[comprimento - 1 - posicao]; // substituiu G por l
        texto[comprimento - 1 - posicao] = auxiliar;
    }  
}

int main()  
{
    char meu_texto[255];
    printf ("Insira um texto: ");
    fgets(meu_texto, 255, stdin);

    printf ("Antes de inverter o texto:\n%s\n", meu_texto);
    inverte(meu_texto);
    printf ("Após inverter o texto: %s", meu_texto);
}
