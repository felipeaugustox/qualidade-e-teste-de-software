# Códigos qualidade e teste de software

### Aula 1: Exercício entrada x saída de dados com .txt

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

### Aula 2: Introdução ao JUnit ~no modo root~ sem IDE

##### Compilando e executando o projeto:

Compilando:
```
javac src/Calculator.java
javac -cp .;libs/junit-4.xx.jar;libs/hamcrest-core-1.3.jar src/CalculatorTests.java
```

Executando:
```
java -cp .;libs/junit-4.xx.jar;libs/hamcrest-core-1.3.jar org.junit.runner.JUnitCore src.CalculatorTests
```
