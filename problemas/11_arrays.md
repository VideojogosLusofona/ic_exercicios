# Arrays e apontadores

1 - Completa o código da seguinte função, cujo objectivo é fazer uma soma de
dois _arrays_, guardando o resultado no primeiro _array_. A variável `tamanho`
representa o tamanho dos _arrays_.

```c
void soma_arrays(int *array1, int *array2, int tamanho) {
    /* Inserir codigo aqui */
}
```

> [Soluções](../solucoes/11_arrays/01.md)

2 - No código seguinte as duas primeiras instruções definem três variáveis: um
_array_ e dois apontadores. As instruções seguintes representam várias
operações sobre essas variáveis. Indica quais dessas instruções são inválidas e
justifica a tua resposta.

```c
/* Variaveis */
unsigned char a[4] = {10, 20, 30, 40, 50};
int *puc;
void *pg;

/* Instrucoes a verificar: */
puc = a;
pg = a;
puc[3]++;
pg = puc;
pg[2] = 0;
puc[2] = 0;
a[5] = 60;
--puc;
pg++;
puc = pg;
a = puc;
*(puc + 2) = 31;
*(a + 3) = 41;
*(pug + 1) = 21;
```

> [Soluções](../solucoes/11_arrays/02.md)

3 - A variável `p` é um apontador para `long`, apontando inicialmente para o
endereço de memória 0x9F88. Qual o valor de `p` após a operação `p += 2`
assumindo que variáveis do tipo `long` têm 64 bits? Explica o teu raciocínio.

> [Soluções](../solucoes/11_arrays/03.md)

4 - Indica o que é impresso no ecrã pelo seguinte programa, explicando o que
fazem cada uma das instruções entre os comentários `START` e `END`:

```c
#include <stdio.h>
#include <stdlib.h>
#define ARRSIZE 5
int main() {

    int a[ARRSIZE] = {4, 2, 1, 5, 1};
    int b[ARRSIZE] = {-1, -2, 0, -4, -3};
    int *pa = a;
    int *pb = b;

    /* START */
    *(pa + 2) *= 2;
    pb[1] = *a * 3;
    *(a + 1) &= pb[3];
    *(b + 4) <<= *(pa + 4);
    *pa %= pa[3];
    pb++;
    pb[0] *= b[1];
    /* END */

    for (int i = 0; i < ARRSIZE; i++) {
        printf("%d %d\n", a[i], b[i]);
    }

    return 0;
}
```

> [Soluções](../solucoes/11_arrays/04.md)
