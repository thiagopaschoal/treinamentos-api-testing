# **Testes de API (API Testing) - Java I (Conceitos Básicos)**

*Thiago Sakurai Paschoal*

Tabela de conteúdos
=================
<!--ts-->

* [O que precisamos ter no nosso cinto de utilidades antes de começar?](#cinto-utilidades)
* [Instalando o ambiente Java](#ambiente-java)
* [Instalando e configurando o Eclipse](#ambiente-eclipse)
* [Criando e executando nosso primeiro programa Java](#criando-executando-projeto)
* [Criando dados para nosso programa (Variáveis)](#variaveis)
* [Dando poder de decisão para nosso programa](#estruturas)
* [Falando um pouco sobre classes e objetos](#oo)
* [Exercicios](EXERCICIOS.md)

<!--te-->

<h3 id="cinto-utilidades">
    <strong>O que precisamos ter no nosso cinto de utilidades antes de começar?</strong>
</h3>

Antes de começar, aviso de que este é um treinamento proibido para menores de 18 anos e que este só devem assistir acompanhados dos pais/responsáveis. **Brincadeiraaaa!!!!**. Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:

1. JDK (8)

2. Eclipse

**O que é JDK? JVM? JRE?**
<br>
<h4 id="ambiente-java">
    <strong>Instalando o ambiente Java</strong>
</h4>
<h4> 
	🚧  Instalando o ambiente Java 🚀 Em construção...  🚧
</h4>
<br>

<h4 id="ambiente-eclipse">
    <strong>Instalando e configurando o Eclipse</strong>
</h4>

<h4> 
	🚧  Instalando e configurando o Eclipse 🚀 Em construção...  🚧
</h4>
<br>

<h3 id="criando-executando-projeto">
    <strong>Criando e executando nosso primeiro programa Java</strong>
</h3>

Neste capítulo do nosso treinamento, vamos iniciar o desenvolvimento do nosso primeiro projeto. Vamos começar com algo simple, bem simples mas que nós trás bastantes insights e explicações. Todos nos já passamos pelo bom e velho ***Hello-World***.

```java
public class MeuPrimeiroProgramaJava {
    public static void main (String[] args) {
        System.out.println("Hello World");
    }
}
```

#### ***Criando o projeto no Eclipse***
<h4> 
	🚧  Criando o projeto no Eclipse 🚀 Em construção...  🚧
</h4>
<br>
#### ***Executando o projeto no Eclipse***
<h4> 
	🚧  Executando o projeto no Eclipse 🚀 Em construção...  🚧
</h4>
<br>

<h3 id="variaveis">
    <strong>Criando dados para nosso programa (Variáveis)</strong>
</h3>

- ***Qual a motivação em declarar uma variável?***
- ***Como declarar?***
- ***Quais os tipos possíveis de variáveis/atributos em Java?***
- ***Eu posso mudar converter um tipo para outro?***

Dentro de um bloco, podemos declarar variáveis e usá-las. Em Java, toda variável tem um tipo que não pode ser mudado uma vez declarado:

```code
tipoDaVariavel nomeDaVariavel;
```

| Tipos | Tamanho |
| ----------- | ----------- |
| boolean | 1 bit |
| byte | 1 byte | 
| char | 2 bytes | 
| short | 2 bytes | 
| int | 4 bytes | 
| float | 4 bytes | 
| long | 8 bytes | 
| double | 8 bytes | 

```java
int idade = 18;
String mensagemEsperada = "Sistema Indisponível";
char sexo = 'M';
boolean hasAttributes = true;
double pi = 3.14;
boolean menorDeIdade = idade < 18;
double x = 5 * 10;
```

- ***Operadores Aritméticos***
    -   `+` (Soma/Concatenação)
    ```java
    int valor = 19;
    int resultado = valor + 2;
    System.out.println(resultado); // 21
    ```

    -   `-` (Subtração)
    ```java
    int valor = 10;
    int resultado = valor - 2;
    System.out.println(resultado); // 5
    ```
    -   `*` (Multiplicação)
    ```java
    int valor = 5;
    int resultado = valor * 2;
    System.out.println(resultado); // 10
    ```
    -   `/` (Divisão)
    ```java
    int valor = 4;
    int resultado = valor / 2;
    System.out.println(resultado); // 2
    ```
    -  `%` (Resto)

    ```java
    int valor = 4;
    boolean ehPar = valor % 2 == 0;
    System.out.println(ehPar); // true
    ```

    ### ***CUIDADO***

    Quando estamos usando o operador de soma entre texto, por mais que o valor do texto seja um número o resultado será apenas a junção de ambos:

    ```java
    String valor = "20";
    String resultado = valor + 2;
    System.out.println(resultado); // 202
    ```
- ***Operadores Relacionais***
    -   `==` (Igual/Comparaçao)
    ```java
    double valor = 3.14;
    boolean resultado = valor == 3;
    System.out.println(resultado); // false
    ```
    -   `!=` (Diferente)
    ```java
    double valor = 3.14;
    boolean resultado = valor != 3;
    System.out.println(resultado); // true
    ```
    -   `>` (Maior)
    ```java
    double valor = 89;
    boolean resultado = valor > 100;
    System.out.println(resultado); // false
    ```
    -   `<` (Menor)
    ```java
    double valor = 89;
    boolean resultado = valor < 100;
    System.out.println(resultado); // true
    ```
    -  `>=` (Maior ou igual)
    ```java
    double valor = 3;
    boolean resultado = valor >= 3;
    System.out.println(resultado); // true
    ```
    ```java
    double valor = 1;
    boolean resultado = valor >= 3;
    System.out.println(resultado); // false
    ```
    ```java
    double valor = 17;
    boolean resultado = valor >= 3;
    System.out.println(resultado); // true
    ```
    -  `<=` (Menor ou igual)
    ```java
    double valor = 4;
    boolean resultado = valor <= 3;
    System.out.println(resultado); // false
    ```
    ```java
    double valor = 1;
    boolean resultado = valor <= 3;
    System.out.println(resultado); // true
    ```
- ***Operadores Lógicos***
    -   `&&` (E)
    ```java
    boolean podeDirigir = true;
    boolean podeBeber = idade >= 18;
    boolean resultado = podeDirigir && podeBeber;
    System.out.println(resultado); // true
    ```
    -   `||` (OU)
    ```java
    boolean erroStatusCode = 404;
    boolean resultado = erro == 404 || erro == 400;
    System.out.println(resultado); // true
    ```

<h3 id="estruturas">
    <strong>Dando poder de decisão para nosso programa</strong>
</h3>

- ***if-else***

    - No Java, a sintaxe do if-else é a seguinte:

    ```java
    if (condicaoBooleana) {
        codigo;
    }
    ```
    Uma condição booleana é qualquer expressão que retorne true ou false. Para isso, você pode usar os operadores <, >, <=, >= e operadores lógicos. Um exemplo:

    ```java
    int idade = 15;
    if (idade < 18) {
        System.out.println("Não pode entrar");
    }
    ```

    Além disso, você pode usar a cláusula else para indicar o comportamento que deve ser executado no caso da expressão booleana ser falsa:

    ```java
    int idade = 15;
    if (idade < 18) {
        System.out.println("Não pode entrar");
    } else {
        System.out.println("Pode entrar");
    }
    ```

- ***switch***

    - No Java, a sintaxe do switch é a seguinte:

    ```java
    switch (valor) {
        case valores:
        // o que fazer
        break;
        default:
            // caso default
    }
    ```

    Para demonstrar o uso do switch, vamos criar uma simple ***Calculdora***.

    ```java
    char operador = '+';
    int numero1 = 4;
    int numero2 = 8;
    double resultado = 0D;
    switch (operador) {
        case '+':
        resultado = numero1 + numero2;
        break;
        case '-':
        resultado = numero1 * numero2;
        break;
        case '*'
        resultado = numero1 * numero2;
        break;
        case '/':
        resultado = numero1 / numero2;
        break;
        default:
            System.out.println("operador inválido");
    }
    ```

- ***while***

    - O while é um comando usado para fazer um laço (loop), isto é, repetir um trecho de código algumas vezes. A ideia é que esse trecho de código seja repetido enquanto uma determinada condição permanecer verdadeira.

        ```java
        while (expressao-booleana) {
            // execute e pare quando a condiçao for falsa
        }
        ```

        Para demonstrar o uso do while, vamos criar uma simples ***Tabuada***.

        ```java
        int valor = 4;
        int counter = 0;
        while (counter <= 10) {
            System.out.println(valor + "*" + counter + "=" + (valor*counter));
            counter++;
        }
        ```

- ***for***

    - Outro comando de loop extremamente utilizado é o for. A ideia é a mesma do while: fazer um trecho de código ser repetido, enquanto uma condição continuar verdadeira. Mas, além disso, o for isola também um espaço para inicialização de variáveis e o modificador dessas variáveis. Isso faz com que as variáveis relacionadas ao loop fiquem mais legíveis:

        No Java, a estrutura do for é a seguinte:

        ```java
        for (inicializacao; condicao; incremento) {
            // codigo;
        }
        ```

        Vamos adaptar o exemplo da ***Tabuada*** do exemplo anterior para usar o ***for***

        ```java
        int valor = 4;
        for (int i = 0; i <= 10; i++) {
            System.out.println(valor + "*" + i + "=" + (valor*i));
        }
        ```

<h3 id="oo">
    <strong>Falando um pouco sobre classes e objetos</strong>
</h3>

- 4 pilares da Orientação de Objetos

    - Abstração
    - Encapsulamento
    - Herança
    - Polimorfismo

- Vamos tomar como exemplo, uma classe de nome ***Conta***.

```java
public class Conta {
    
    private String titular;
    private Long cpf;
    private Double saldo;
    // .. outros atributos

    public void sacar(dobule valor) {
        this.saldo -= valor;
    }

    public void deposita(double valor) {
        this.saldo += valor;
    }

    // ..outros comportamentos

    public Double getSaldo() {
        return this.saldo;
    }

    public Long getCpf() {
        return this.cpf;
    }

    public String getTitular() {
        return this.titular;
    }
}
```

Ao projeto da conta, isto é, à definição da conta, damos o nome de classe. Ao que podemos construir a partir desse projeto; às contas de verdade, damos o nome de objetos.

