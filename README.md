# geradorHexForBFA

Esse programa tem por objetivo gerar um txt de todas as possibilidades de chaves hexadecimais, contendo até 32b bits.

char caracter1 = 0;
char caracter2 = 0;
char caracter3 = 0;
.
.
.


Aqui algo de estranho acontece; 
Eu sei que para representar números usa-se “int”, no entanto, como o int ocupa mais espaço e requer mais processamento, e esse programa roda laços “for” aninhados, usar o int tornou-se um problema.
 A solução foi passar para “char”, é uma variável de menor tamanho, eu penso que não deveria funcionar as expressões relacionais, mas funciona, e a saída é confiável e assim foi possível reduzir o processamento, gerando uma produção mais rápida da tabela. 

char caractere1 = 0;

for(cactere1 = 0X0; caractere1 <= 0XF; caractere1++) //isso funciona…
{
	printf(“%X”, caractere1);
}
