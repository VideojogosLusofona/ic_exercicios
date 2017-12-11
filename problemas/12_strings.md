# Strings

1 - Completa o código da seguinte função, cujo objectivo é converter todos os
espaços numa string em underscores. Por exemplo, a string "Bem vindo a Lisboa!"
seria transformada em "Bem_vindo_a_Lisboa".

```c
void subst_espacos_por_underscores(char *string)
{
    /* Codigo aqui. */
}
```

> [Soluções](../solucoes/12_strings/01.md)

2 - Completa o código da seguinte função, cujo objectivo é contar o número de
caracteres existentes numa string (ou seja, determinar o comprimento da string).

```c
void comprimento_string(char *string)
{
    /* Codigo aqui. */
}
```

> [Soluções](../solucoes/12_strings/02.md)

3 - Completa o código da seguinte função, cujo objectivo é comparar se duas
strings são iguais, independentemente de minúsculas e maiúsculas. Por exemplo,
a função deve devolver 1 (`TRUE`) para as strings "Ola" e "OLA", mas deve
devolver 0 (`FALSE`) para as strings "Ola" e "Ole".

```c
void compara_strings_indep_maiusc(char *str1, char *str2)
{
    /* Codigo aqui. */
}
```

> [Soluções](../solucoes/12_strings/03.md)

4 - Completa o código da função `quantas_vezes`, cujo objectivo é devolver o
número de vezes que determinado carácter (dado pela variável `c`) ocorre numa
string. Por exemplo, a chamada `quantas_vezes("Universidade Lusofona", 'a')
deve devolver 2.

```c
void quantas_vezes(char *string, char c)
{
    /* Codigo aqui. */
}
```

> [Soluções](../solucoes/12_strings/04.md)
