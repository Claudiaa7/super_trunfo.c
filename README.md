# super_trunfo.c

#include <stdio.h>

int main(){
    // Dados da primeira cidade
    char estado1, codigo1[3], nome1[50];
    long long populacao1;
    float area1, pib1;
    int pontosTuristicos1;

    // Dados da segunda cidade
    char estado2, codigo2[3], nome2[50];
    long long populacao2;
    float area2, pib2;
    int pontosTuristicos2;

     // Entrada de dados para a cidade 1
     printf("Digite o estado da cidade 1: ");
     scanf(" %c", &estado1);
     printf("Digite o código da cidade 1: ");
     scanf(" %s", codigo1);
     printf("Digite o nome da cidade 1: ");
     scanf(" %[^\n]", nome1);
     printf("Digite a população da cidade 1: ");
     scanf("%lld", &populacao1);
     printf("Digite a área da cidade 1 (em km²): ");
     scanf("%f", &area1);
     printf("Digite o PIB da cidade 1 (em bilhões de reais): ");
     scanf("%f", &pib1);
     printf("Digite o número de pontos turísticos da cidade 1: ");
     scanf("%d", &pontosTuristicos1);

     // Entrada de dados para a cidade 2
    printf("\nDigite o estado da cidade 2: ");
    scanf(" %c", &estado2);
    printf("Digite o código da cidade 2: ");
    scanf(" %s", codigo2);
    printf("Digite o nome da cidade 2: ");
    scanf(" %[^\n]", nome2);
    printf("Digite a população da cidade 2: ");
    scanf("%lld", &populacao2);
    printf("Digite a área da cidade 2 (em km²): ");
    scanf("%f", &area2);
    printf("Digite o PIB da cidade 2 (em bilhões de reais): ");
    scanf("%f", &pib2);
    printf("Digite o número de pontos turísticos da cidade 2: ");
    scanf("%d", &pontosTuristicos2);

     // Cálculos para a cidade 1
     float densidade1 = populacao1 / area1;
     float pibPerCapita1 = (pib1 * 1e9) / populacao1; // PIB em reais dividido pela população
 
     // Cálculos para a cidade 2
     float densidade2 = populacao2 / area2;
     float pibPerCapita2 = (pib2 * 1e9) / populacao2; // PIB em reais dividido pela população

     // Exibição dos resultados para a cidade 1
    printf("\nCarta 1:\n");
    printf("Estado: %c\n", estado1);
    printf("Código: %s\n", codigo1);
    printf("Nome da Cidade: %s\n", nome1);
    printf("População: %lld\n", populacao1);
    printf("Área: %.2f km²\n", area1);
    printf("PIB: %.2f bilhões de reais\n", pib1);
    printf("Número de Pontos Turísticos: %d\n", pontosTuristicos1);
    printf("Densidade Populacional: %.2f hab/km²\n", densidade1);
    printf("PIB per Capita: %.2f reais\n", pibPerCapita1);
}
