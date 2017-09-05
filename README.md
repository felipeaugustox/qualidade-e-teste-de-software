# Qualidade e teste de software

## 1: Exercício entrada x saída de dados com .txt

> Faça um programa que leia a partir de um arquivo texto, a velocidade do trem A, a velocidade do trem B e uma distância entre dois trens. Calcule e compare com as saídas do arquivo texto, o tempo em que os trens se encontrarão (Equação A), a distância percorrida pelo trem A (Equação B) e a distância percorrida pelo trem B (seguindo a mesma lógica utilizada pelo trem A).

```math
tempo = distância/(velocidade A + velocidade B)
distancia A = tempo * velocidade A
distancia B = tempo * velocidade B
```

* Classes utilizadas
  * BufferedReader
  * FileReader
  * IOException
  * File
  * BigDecimal
  * RoundingMode

## 2: Introdução ao JUnit ~no modo root~ sem IDE

#### Compilando e executando o projeto:

Compilando no Linux ou MacOS:
```
javac src/Calculator.java
javac -cp .:libs/junit-4.xx.jar:libs/hamcrest-core-1.3.jar src/CalculatorTests.java
```
Compilando no Windows:
```
javac src/Calculator.java
javac -cp .;libs/junit-4.xx.jar;libs/hamcrest-core-1.3.jar src/CalculatorTests.java
```
Executando no Linux ou MacOS:
```
java -cp .:libs/junit-4.xx.jar:libs/hamcrest-core-1.3.jar org.junit.runner.JUnitCore src.CalculatorTests
```
Executando no Windows:
```
java -cp .;libs/junit-4.xx.jar;libs/hamcrest-core-1.3.jar org.junit.runner.JUnitCore src.CalculatorTests
```
:exclamation: Lembre-se de substituir o "xx" pela sua versão do junit e inseri-los na pasta adequada (ou alterar os caminhos nos comandos).

## 3: Testes unitários e mais alguns tópicos estudados (É possível rodar com o .bat no Windows)

Tópicos estudados do artigo [DevMedia](http://www.devmedia.com.br/junit-implementando-testes-unitarios-em-java-parte-i/1432):

#### Extreme Programming (XP)
![alt tag](http://ronjeffries.com/xprog/what-is-extreme-programming/circles.jpg)

#### TDD - Test Driven Development
![alt tag](https://upload.wikimedia.org/wikipedia/commons/0/0b/TDD_Global_Lifecycle.png)

#### Testes unitários
O teste unitário é uma modalidade de testes que se concentra na verificação da menor unidade do projeto de software. É realizado o teste de uma unidade lógica, com uso de dados suficientes para se testar apenas à lógica da unidade em questão.
![alt tag](http://3.bp.blogspot.com/-Y2JUPHMLpcE/U8zltJgQRwI/AAAAAAAAWkg/R7OUXJY7GdY/s1600/Chuck+Norris+can+unit+test+entire+applications+with+a+single+assert.jpg)

#### Testes unitários com XP
![alt tag](http://www.devmedia.com.br/imagens/javamagazine/mpjuiiujfig03.jpg)

#### A lista abaixo exemplifica bem como você pode planejar e executar seus testes:

1.  Defina uma lista de tarefas a implementar (o que testar).

2.  Escreva uma classe (test case) e implemente um método de teste para uma tarefa da lista.

3.  Rode o JUnit e certifique-se que o teste falha.

4.  Implemente o código mais simples que rode o teste.

5.  Refatore o código para remover a duplicação de dados.

6.  Caso necessário, escreva mais um teste ou refine o existente.

7.  Faça esses passos para toda a lista de tarefas.

## 4:
