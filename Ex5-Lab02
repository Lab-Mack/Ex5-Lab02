#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int sortear_numero() {
    srand(time(NULL));
    return (rand() % 100) + 1;
}

int ler_palpite() {
    int palpite;
    do {
        printf("Digite seu palpite (1 a 100): ");
        scanf("%d", &palpite);
        if (palpite < 1 || palpite > 100)
            printf("Valor invalido! Digite um numero entre 1 e 100.\n");
    } while (palpite < 1 || palpite > 100);
    return palpite;
}

void verificar_palpite(int palpite, int sorteado) {
    if (palpite == sorteado)
        printf("Parabens!!! Voce acertou!\n");
    else if (palpite < sorteado)
        printf("Voce chutou muito baixo! O valor correto e %d.\n", sorteado);
    else
        printf("Voce chutou muito alto! O valor correto e %d.\n", sorteado);
}

int main() {
    int sorteado = sortear_numero();
    int palpite = ler_palpite();
    verificar_palpite(palpite, sorteado);
    return 0;
}
