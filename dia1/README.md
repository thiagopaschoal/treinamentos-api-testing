<h1 align="center">Java I (Conceitos Básicos)</h1>
<p align="center">Thiago Sakurai Paschoal</p>

Tabela de conteúdos
=================
<!--ts-->

* [O que precisamos ter no nosso cinto de utilidades antes de começar?](#cinto-utilidades)
* [Instalando o ambiente Java](#ambiente-java)
* [Instalando e configurando o Eclipse](capitulos/03.md)
* [Criando e executando nosso primeiro programa Java](capitulos/04.md)
* [Criando dados para nosso programa (Variáveis)](capitulos/05.md)
* [Dando poder de decisão para nosso programa](capitulos/06.md)
* [Falando um pouco sobre classes e objetos](capitulos/07.md)
* [Exercicios](capitulos/08.md)

<!--te-->

<h3 id="cinto-utilidades">
    <strong>O que precisamos ter no nosso cinto de utilidades antes de começar?</strong>
</h3>

Antes de começar, aviso de que este é um treinamento proibido para menores de 18 anos e que este só devem assistir acompanhados dos pais/responsáveis. **Brincadeiraaaa!!!!**. Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:

1. [JDK (8)](https://www.oracle.com/br/java/technologies/javase/javase8-archive-downloads.html)

2. [Eclipse](https://www.eclipse.org/downloads/)

**O que é JDK? JVM? JRE?**
<br>
<h4 id="ambiente-java">
    <strong>Instalando o ambiente Java</strong>
</h4>

1. Selecione qual distribuição deseja baixar de acordo com seu sistema operacional.

![distribuicao](screenshots/distribuicao.png)

2. Marque os termos da Oracle (checkbox) e depois clique no botão verde

![download](screenshots/download.png)

3. Para seguir com o download é necessário você ter uma conta Oracle. Caso não tenha, crie uma! Vc não paga nada por isso.

![login](screenshots/login.png)

4. Download realizado com sucesso!

![login](screenshots/download-feito.png)

5. Siga o passo-a-passo do procedimento de instalação (***Next, Next, Next...***)

6. Após finalizar a instalação, nas adicione essas informações nas variáveis de ambiente do seu SO.

    6.1. Digite variáveis na caixa de pesquisa do 'Windows' e depois clique em 'Editar as variáveis de ambiente do sistema'

    ![caminho-env](screenshots/caminho-env.png)

    6.2. Clique em 'Variaveis de Ambiente'

    ![env](screenshots/env.png)

    6.3. Adicione a variavel chamada ***JAVA_HOME*** no grupo 'Variaveis de ambiente'.

    ```code
    JAVA_HOME = C:\Program Files\Java\jdk1.8.0_202
    ```
    ![java-home](screenshots/java_home.png)

    6.4. Depois adicione a mesma variável agora, em conjunto com a variável ***PATH***

    ![path](screenshots/path.png)

    6.5. Reinicie o sistema

    6.6. Após reiniciar, abra o seu terminal (CMD, Windows Terminal etc) e digite:

    ```code
    java -version
    ```
    ![sucesso](screenshots/sucesso.png)

## Excelente, se vc chegou até aqui com sucesso significa que seu ambiente Java está completo!!!! Topzera