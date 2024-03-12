<h1>
    <a href="https://www.oracle.com/java/">
     <img align="center" width="40px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg"></a>
    <span>Java</span>
</h1>

# Linguagem Java

## Convenção de Código

A convenção de código do Java é um conjunto de regras recomendadas para escrever código Java que é fácil de ler, entender e manter. Essas regras foram definidas pela Oracle, a empresa que mantém a linguagem Java, e são amplamente seguidas pela comunidade de desenvolvedores Java.

**Algumas das principais convenções de código do Java**:

Nomes de classes devem começar com letra maiúscula e usar a convenção PascalCase (também conhecida como Upper CamelCase).
- **`MinhaClasse`**.

Nomes de métodos devem começar com letra minúscula e usar a convenção camelCase.
- **`meuMetodo()`**.

Nomes de constantes devem ser totalmente em letras maiúsculas, separadas por underline.
- **`MINHA_CONSTANTE`**.

Nomes de variáveis devem começar com letra minúscula e usar a convenção camelCase.
- **`minhaVariavel`**.

Todas as linhas de código devem ter no máximo 80 caracteres de largura para facilitar a leitura.

Recomenda-se usar espaços em branco para separar operadores, palavras-chave e elementos de controle de fluxo.
- **`if (condicao) {`**.

Use comentários para documentar seu código, explicando o que ele faz e por que ele faz isso. Comentários devem ser claros e concisos.
- Esse ponto é polêmico, pois muitas pessoas desenvolvedoras consideram que um bom código deve ser autoexplicativo. Se você utiliza nomes intuitivos e descritivos para suas variáveis e métodos, fica mais claro de entender o que está acontecendo no código, dispensando a necessidade de uso de comentários.

## Tipos Primitivos

Em Java, assim como na maioria das linguagens de programação, existem os tipos primitivos, que são os tipos de dados mais básicos e fundamentais da linguagem. Eles são utilizados para representar valores simples e são definidos pela própria linguagem.

Java possui oito tipos primitivos diferentes: **`boolean`**, **`byte`**, **`char`**, **`short`**, **`int`**, **`long`**, **`float`** e **`double`**. Cada um desses tipos possui suas próprias características e faixa de valores permitidos.

### boolean

O tipo boolean é utilizado para representar valores lógicos, podendo assumir apenas dois valores: **true** ou **false**. É utilizado em expressões condicionais, loops e outros casos onde se deseja avaliar se uma determinada condição é verdadeira ou falsa.

### byte

O tipo byte é utilizado para representar valores numéricos **inteiros de 8 bits**. Ele possui uma faixa de valores de **-128 a 127**.

### char

O tipo char é utilizado para representar **caracteres individuais**. Ele pode armazenar qualquer **caractere Unicode** e é representado por aspas simples **`('')`**.

### short

O tipo short é utilizado para representar valores numéricos **inteiros de 16 bits**. Ele possui uma faixa de valores de **-32.768 a 32.767**.

### int

O tipo int é utilizado para representar valores numéricos **inteiros de 32 bits**. É um dos tipos de dados mais utilizados para representar números inteiros em Java e possui uma faixa de valores de **-2.147.483.648 a 2.147.483.647**.

### long

O tipo long é utilizado para representar valores numéricos **inteiros de 64 bits**. Ele é utilizado para representar valores inteiros muito grandes e possui uma faixa de valores de **-9.223.372.036.854.775.808 a 9.223.372.036.854.775.807**.

### float

O tipo float é utilizado para representar valores numéricos de **ponto flutuante**, ou seja, **valores com casas decimais**, sendo que ocupa **32 bits** de memória. Ele pode representar números decimais com **até 7 dígitos** e tem uma **precisão limitada**, o que significa que ele **pode arredondar os números se eles forem muito grandes ou muito pequenos**.

### double

O tipo double é similar o float, entretanto ele ocupa **64 bits** de memória e pode representar **números decimais** com **até 15 dígitos**.

## Operadores

### Operadores de Atribuição

Utilizados para atribuir um valor a uma variável. O operador de atribuição básico é o **`"="` (sinal de igual)**.

```java
int valor =  5;  //Atribui o valor 5 à variável valor  
```

Existem também operadores de atribuição combinados, que são uma forma abreviada de atribuição. Por exemplo, o operador **`"+="`** adiciona um valor à variável existente.

```java
int valor =  10; 
valor += 15;  //Equivalente a valor = valor + 15, atribui o valor 25 à variável valor 
```

### Operadores Aritméticos

Os operadores aritméticos são usados para realizar operações matemáticas básicas. São eles:

- **`"+"` (adição)**
- **`"-"` (subtração)**
- **`"*"` (multiplicação)**
- **`"/"` (divisão)**
- **`"%"` (resto da divisão)**

```java
int a = 10 + 5; // Atribui o valor 15 à variável a
int b = 10 - 5; // Atribui o valor 5 à variável b
int c = 10 * 5; // Atribui o valor 50 à variável c
int d = 10 / 5; // Atribui o valor 2 à variável d
int e = 10 % 3; // Atribui o valor 1 à variável e (o resto da divisão de 10 por 3 é 1)
```

### Operadores Relacionais

Os operadores relacionais são usados para comparar valores. Eles retornam um valor booleano (verdadeiro ou falso). São eles:

- **`"=="` (igual a)**
- **`"!="` (diferente de)**
- **`">"` (maior que)**
- **`">="` (maior ou igual a)**
- **`"<"` (menor que)**
- **`"<="` (menor ou igual a)**

```java
int a = 10; // Atribui o valor 10 à variável a
int b = 5; // Atribui o valor 5 à variável b
int c = 30; // Atribui o valor 30 à variável c

boolean igual = (b == a); //Nesse caso a variável igual ficará com o valor *false*, pois o valor de b não é igual o valor de a.
boolean diferente = (b != c); //A variável diferente ficará com o valor *true*, pois o valor de b é diferente do valor de c.
boolean maior = (b > a); //A variável maior ficará com o valor *false*, pois o valor de b é menor que o valor de a.
boolean menorIgual = (b <= c); //A variável menorIgual ficará com o valor *true*, pois o valor de b é menor que o valor de c.
```

### Operadores Lógicos

Esses operadores são usados quando queremos verificar duas ou mais condições e/ou expressões na aplicação. Eles fazem a comparação de valores booleanos e retornam também um resultado booleano.

São três operadores: **`AND (&&)`**, **`OR (||)`** e **`NOT (!)`**.

O operador **`AND (&&)`**, que traduzindo para o português seria o E, é usado para verificar se duas condições são verdadeiras. Se ambas as condições forem verdadeiras, o resultado será verdadeiro. Caso contrário, o resultado será falso.

```java
boolean a = true;
boolean b = false;
if (a && b) {
   // Este código não será executado, já que a é verdadeiro e b é falso.
}
```

O operador **`OR (||)`**, que traduzindo para o português seria o OU, é usado para verificar se pelo menos uma das condições é verdadeira. Se pelo menos uma das condições for verdadeira, o resultado será verdadeiro. Caso contrário, o resultado será falso.

```java
boolean a = true;
boolean b = false;
if (a || b) {
   // Este código será executado, já que a é verdadeiro, mesmo que b seja falso.
}
```

O operador **`NOT (!)`** é usado para negar uma condição. Se a condição for verdadeira, o resultado será falso. Se a condição for falsa, o resultado será verdadeiro.

```java
boolean a = true;
if (!a) {
   // Este código não será executado, já que a é verdadeiro.
}
```
### Operadores de Incremento

O operador de incremento é usado para aumentar o valor de uma variável em 1. Existem dois tipos de operadores de incremento: o operador de **`pré-incremento (++variavel)`** e o operador de **`pós-incremento (variavel++)`**.

O operador de **`pré-incremento (++variavel)`** aumenta o valor da variável em 1 antes de usar a variável em uma expressão.

```java
int num = 5;
int resultado = ++num; //num é incrementado para 6 e depois atribuído a resultado
System.out.println(num); // imprime 6
System.out.println(resultado); // imprime 6
```

Já o operador de **`pós-incremento (variavel++)`** aumenta o valor da variável em 1 depois de usar a variável em uma expressão.

```java
int num = 5;
int resultado = num++; //num é atribuído primeiramente à variável resultado e depois incrementado para 6
System.out.println(num); // imprime 6
System.out.println(resultado); // imprime 5
```

## Strings e Text Blocks

A classe String é responsável por representar uma **sequência de caracteres**, ou seja, **um texto**.

### Criação de Strings

Para criar uma String em Java, basta utilizar **aspas duplas** para delimitar o texto.

```java
String nome = "Alura";
```

É possível concatenar duas ou mais Strings utilizando o operador +.

```java
String saudacao = "Olá, ";
String nome = "Alura";
String mensagem = saudacao + nome + "!";
```

### Comparação de Strings

Em Java, é possível comparar duas Strings utilizando o operador ==. Porém, esse operador verifica apenas se as duas variáveis apontam para o mesmo objeto na memória, e não se o conteúdo das Strings é igual. Para **comparar o conteúdo de duas String**s, é necessário utilizar o método **equals()**.

```java
String senha = "12345";
if (senha.equals("12345")) {
    System.out.println("Acesso autorizado!");
} else {
    System.out.println("Senha incorreta.");
}
```

### Text Block

Introduzido na versão 15 do Java, o Text Block é uma nova forma de representar Strings que facilitam a escrita de textos com múltiplas linhas. Em vez de utilizar aspas duplas para delimitar o texto e inserir quebras de linha manualmente, ou utilizar concatenações, é possível utilizar uma sintaxe mais simples que permite inserir o texto exatamente como ele é.

Para criar um Text Block em Java, basta **utilizar três aspas duplas para delimitar o texto**, seguidas de **uma quebra de linha**.

```java
String mensagem = """
                  Olá, mundo!
                  Este é um Text Block.
                  Ele permite escrever textos com múltiplas linhas
                  sem precisar usar caracteres de escape ou quebras de linha manualmente ou concatenações.
                  """;
```

## Formatação de Textos

Em Java, é possível formatar textos e números de diversas maneiras. Isso pode ser útil em diversas situações, como ao exibir valores para o usuário de uma maneira mais legível.

Uma das maneiras mais comuns de se formatar textos em Java é utilizando o método **format()**, da **classe String**. Esse método permite formatar um texto utilizando diversos placeholders, que são representados pelo caractere **% seguido de uma letra que indica o tipo de dado que será inserido** no placeholder. Por exemplo, **`%s` indica que uma String** será inserida no placeholder, **`%d` indica um valor inteiro** e **`%f` indica um valor de ponto flutuante**.

```java
String nome = "Maria";
int idade = 30;
double valor = 55.9999;
System.out.println(String.format("Meu nome é %s, eu tenho %d anos e hoje gastei %.2f reais", nome, idade, valor));
```

## Casting

Casting é um recurso utilizado em Java para converter um tipo de dado em outro. Essa conversão pode ser feita de forma **automática pelo compilador (conversão implícita)**, quando o **tipo de dado de destino é compatível com o tipo de dado de origem**, ou de forma **manual (conversão explícita)**, utilizando o **operador de casting**.

### Casting Implícito

O casting implícito é realizado **automaticamente pelo compilador** quando o **tipo de dado de origem é compatível com o tipo de dado de destino**.

```java
int x = 10;
double y = x; // casting implícito
```

### Casting Explícito

O casting explícito é realizado quando o **tipo de dado de origem é incompatível com o tipo de dado de destino**. Nesse caso, devemos **utilizar o operador de casting** para realizar a conversão:

```java
double x = 10.5;
int y = (int) x; // casting explícito
```

![](https://caelum-online-public.s3.amazonaws.com/2858-java-criando-primeira-aplicacao/imagem21.png)

## Referências
**N/A**