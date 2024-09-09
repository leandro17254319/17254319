//EXERCICIOS
// 1)A)

# include <stdio.h>
int main () {
 long long n = 4000000000;
 printf ("%lld\n", n );
 return 0;
}

//B)
# include <stdio.h>
int main () {
 int a = 0; // initialize a with some value
 printf ("%d\n", a );
 return 0;
}

//C)
# include <stdio.h>
int main () {
 printf ("%d\n", 4);
 printf ("%d\n", 2);
 return 0;
}

//D)
# include <stdio.h>
int main () {
 int a ;
 scanf ("%d", &a );
 printf ("%d\n", a );
 return 0;
}

//2)A)
#include <stdio.h>
int main() {
 int a, b, c;
 // LEIA OS NUMEROS
 printf("Insira o primeiro numero: ");
 scanf("%d", &a);
 printf("Insira o segundo numero: ");
 scanf("%d", &b);
 printf("Insira o terceiro numero: ");
 scanf("%d", &c);
 // IMPRIMA OS NUMEROS NA ORDEM INVERSA
 printf("Os numeros na ordem inversa: %d %d %d\n", c, b, a);
 return 0;
}

//B)
#include <stdio.h>
#include <string.h>
int main() {
 char name[50]; // array para armazenar o nome do usuário
 // Mensagem inicial
 printf("Olá eu sou o Nº 1, como é seu nome? ");
 // Ler o nome do usuario
 scanf("%49s", name); // deixe um espaço para o terminador nulo
 // Mensagem
 printf("Bem-vindo ao clube %s.\n", name);
 return 0;
}


//C)
#include <stdio.h>
int main() {
 char nome[50]; // array para armazenar o nome do usuário
 int idade; // variável para armazenar a idade do usuário
 int dias_vividos; // variável para armazenar o número aproximado de dias vividos
 // Pergunte pelo nome do usuário
 printf("Olá, qual é seu nome? ");
 scanf("%49s", nome); // deixe um espaço para o terminador nulo
 // Pergunte pela idade do usuário
 printf("E qual é sua idade? ");
 scanf("%d", &idade);
 // Calcule o número aproximado de dias vividos
 dias_vividos = idade * 365; // suponha 365 dias por ano (ignorando anos bissextos)
 // Imprima o resultado
 printf("Olá, %s! Você já viveu aproximadamente %d dias.\n", nome, dias_vividos);
 return 0;
}


//D)
#include <stdio.h>
#include <math.h>
int main() {
 float raio; // variável para armazenar o raio do círculo
 float area; // variável para armazenar a área do círculo
 // Pergunte pelo raio do círculo
 printf("Qual é o raio do círculo? ");
 scanf("%f", &raio);
 // Calcule a área do círculo
 area = M_PI * pow(raio, 2);
 // Imprima o resultado
 printf("A área do círculo é aproximadamente %.2f unidades quadradas.\n", area);
 return 0;
}


//E)
#include <stdio.h>
int main() {
 float largura; // variável para armazenar a largura da parede em metros
 float altura; // variável para armazenar a altura da parede em metros
 float area; // variável para armazenar a área da parede em metros quadrados
 float quantidade_tinta; // variável para armazenar a quantidade de tinta necessária em litros
 int latas_necessarias; // variável para armazenar a quantidade de latas necessárias
 // Pergunte pela largura da parede
 printf("Qual é a largura da parede em metros? ");
 scanf("%f", &largura);
 // Pergunte pela altura da parede
 printf("Qual é a altura da parede em metros? ");
 scanf("%f", &altura);
 // Calcule a área da parede
 area = largura * altura;
 // Calcule a quantidade de tinta necessária em litros
 quantidade_tinta = area * 0.3; // 300 ml/m² = 0.3 L/m²
 // Calcule a quantidade de latas necessárias
 latas_necessarias = (int) ceil(quantidade_tinta / 2); // 2 L/lata arredondando para cima usando a função ceil.
 // Imprima o resultado
 printf("Você precisará de aproximadamente %d latas de tinta para pintar a parede.\n", latas_necessarias);
 return 0;
}



//F)
#include <stdio.h>
int main() {
 float farenheit; // variável para armazenar a temperatura em graus Farenheit
 float centigrados; // variável para armazenar a temperatura em graus Centígrados
 // Pergunte pela temperatura em graus Farenheit
 printf("Qual é a temperatura em graus Farenheit? ");
 scanf("%f", &farenheit);
 // Calcule a temperatura em graus Centígrados
 centigrados = (5.0/9.0) * (farenheit - 32.0);
 // Imprima o resultado
 printf("A temperatura em graus Centígrados é aproximadamente %.2f°C.\n", centigrados);
 return 0;
}



//G)
#include <stdio.h>
int main() {
 float pressao; // variável para armazenar a pressão do pneu em libras por polegada quadrada (psi)
 float volume; // variável para armazenar o volume do pneu em pés cúbicos (ft³)
 float temperatura; // variável para armazenar a temperatura do pneu em graus Fahrenheit (°F)
 float massa_ar; // variável para armazenar a massa de ar do pneu em libras (lb)
 // Pergunte pela pressão do pneu
 printf("Qual é a pressão do pneu em psi? ");
 scanf("%f", &pressao);
 // Pergunte pelo volume do pneu
 printf("Qual é o volume do pneu em ft³? ");
 scanf("%f", &volume);
 // Pergunte pela temperatura do pneu
 printf("Qual é a temperatura do pneu em °F? ");
 scanf("%f", &temperatura);
 // Calcule a massa de ar do pneu
 massa_ar = (pressao * volume) / (0.37 * (temperatura + 460));
 // Imprima o resultado
 printf("A massa de ar do pneu é aproximadamente %.2f lb.\n", massa_ar);
 return 0;
}


//H)
#include <stdio.h>
int main() {
 int primeiro_termo; // variável para armazenar o primeiro termo da PA
 int razao; // variável para armazenar a razão da PA
 int n; // variável para armazenar o número N
 int termo_n; // variável para armazenar o N-ésimo termo da PA
 // Pergunte pelo primeiro termo da PA
 printf("Qual é o primeiro termo da PA? ");
 scanf("%d", &primeiro_termo);
 // Pergunte pela razão da PA
 printf("Qual é a razão da PA? ");
 scanf("%d", &razao);
 // Pergunte pelo número N
 printf("Qual é o valor de N? ");
 scanf("%d", &n);
 // Calcule o N-ésimo termo da PA
 termo_n = primeiro_termo + (n - 1) * razao;
 // Imprima o resultado
 printf("O %d-ésimo termo da PA é %d.\n", n, termo_n);
 return 0;
}


//I)
#include <stdio.h>
int main() {
 int primeiro_termo; // variável para armazenar o primeiro termo da PA
 int razao; // variável para armazenar a razão da PA
 int n; // variável para armazenar o número N
 int termo_n; // variável para armazenar o N-ésimo termo da PA
 // Pergunte pelo primeiro termo da PA
 printf("Qual é o primeiro termo da PA? ");
 scanf("%d", &primeiro_termo);
 // Pergunte pela razão da PA
 printf("Qual é a razão da PA? ");
 scanf("%d", &razao);
 // Pergunte pelo número N
 printf("Qual é o valor de N? ");
 scanf("%d", &n);
 // Calcule o N-ésimo termo da PA
 termo_n = primeiro_termo + (n - 1) * razao;
 // Imprima o resultado
 printf("O %d-ésimo termo da PA é %d.\n", n, termo_n);
 return 0;
}



//J)
#include <math.h>
int main() {
 float a, b, c; // variáveis para armazenar os coeficientes da equação de segundo grau
 float delta; // variável para armazenar o discriminante da equação
 float x1, x2; // variáveis para armazenar as raízes da equação
 // Pergunte pelos coeficientes da equação de segundo grau
 printf("Qual é o valor de a? ");
 scanf("%f", &a);
 printf("Qual é o valor de b? ");
 scanf("%f", &b);
 printf("Qual é o valor de c? ");
 scanf("%f", &c);
 // Calcule o discriminante da equação
 delta = b * b - 4 * a * c;
 // Verifique se a equação tem raízes reais
 if (delta >= 0) {
 // Calcule as raízes da equação
 x1 = (-b + sqrt(delta)) / (2 * a);
 x2 = (-b - sqrt(delta)) / (2 * a);
 // Imprima as raízes da equação
 printf("As raízes da equação são x1 = %.2f e x2 = %.2f.\n", x1, x2);
 } else {
 // Imprima uma mensagem de erro se a equação não tiver raízes reais
 printf("A equação não tem raízes reais.\n");
 }
 return 0;
}




//J)
#include <stdio.h>
int main() {
 int quantidade_1_real, quantidade_10_reais, quantidade_50_reais, quantidade_100_reais;
 float valor_total;
 // Pergunte pela quantidade de notas de cada valor
 printf("Quantas notas de 1 real você tem? ");
 scanf("%d", &quantidade_1_real);
 printf("Quantas notas de 10 reais você tem? ");
 scanf("%d", &quantidade_10_reais);
 printf("Quantas notas de 50 reais você tem? ");
 scanf("%d", &quantidade_50_reais);
 printf("Quantas notas de 100 reais você tem? ");
 scanf("%d", &quantidade_100_reais);
 // Calcule o valor total
 valor_total = quantidade_1_real * 1 + quantidade_10_reais * 10 + quantidade_50_reais * 50 + quantidade_100_reais * 100;
 // Imprima o valor total
 printf("O valor total em dinheiro é R$ %.2f.\n", valor_total);
 return 0;
}


//L)
#include <stdio.h>
int main() {
 float valor_total;
 int quantidade_100_reais, quantidade_50_reais, quantidade_10_reais, quantidade_5_reais, quantidade_1_real;
 // Pergunte pelo valor total em dinheiro
 printf("Qual é o valor total em dinheiro? R$ ");
 scanf("%f", &valor_total);
 // Calcule a quantidade de notas de cada valor
 quantidade_100_reais = (int) valor_total / 100;
 valor_total -= quantidade_100_reais * 100;
 quantidade_50_reais = (int) valor_total / 50;
 valor_total -= quantidade_50_reais * 50;
 quantidade_10_reais = (int) valor_total / 10;
 valor_total -= quantidade_10_reais * 10;
 quantidade_5_reais = (int) valor_total / 5;
 valor_total -= quantidade_5_reais * 5;
 quantidade_1_real = (int) valor_total;
 // Imprima a quantidade de notas de cada valor
 printf("Para compor este valor, você precisará de:\n");
 printf("%d nota(s) de 100 reais\n", quantidade_100_reais);
 printf("%d nota(s) de 50 reais\n", quantidade_50_reais);
 printf("%d nota(s) de 10 reais\n", quantidade_10_reais);
 printf("%d nota(s) de 5 reais\n", quantidade_5_reais);
 printf("%d nota(s) de 1 real\n", quantidade_1_real);
 return 0;
}




//Desafio
#include <stdio.h>
int main() {
 float valor_total = 1000.0; // Valor total a ser aportado
 float preco_medio_acao1 = 24.13;
 float preco_medio_acao2 = 11.00;
 float preco_medio_acao3 = 38.65;
 float dividendo_acao1 = 17.00;
 float dividendo_acao2 = 35.00;
 float dividendo_acao3 = 25.00;
 int quantidade_acao1, quantidade_acao2, quantidade_acao3;
 // Calcule a quantidade de ações que podem ser compradas com o valor total
 quantidade_acao1 = (int) (valor_total / preco_medio_acao1);
 quantidade_acao2 = (int) (valor_total / preco_medio_acao2);
 quantidade_acao3 = (int) (valor_total / preco_medio_acao3);
 // Calcule o Dividend Yield (D.Y) de cada ação
 float dy_acao1 = (dividendo_acao1 / preco_medio_acao1) * 100;
 float dy_acao2 = (dividendo_acao2 / preco_medio_acao2) * 100;
 float dy_acao3 = (dividendo_acao3 / preco_medio_acao3) * 100;
 // Imprima os resultados
 printf("Você pode comprar:\n");
 printf("%d ação(ões) da Ação 1\n", quantidade_acao1);
 printf("%d ação(ões) da Ação 2\n", quantidade_acao2);
 printf("%d ação(ões) da Ação 3\n", quantidade_acao3);
 printf("\nO Dividend Yield (D.Y) de cada ação é:\n");
 printf("Ação 1: %.2f%%\n", dy_acao1);
 printf("Ação 2: %.2f%%\n", dy_acao2);
 printf("Ação 3: %.2f%%\n", dy_acao3);
 return 0;
}
