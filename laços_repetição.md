
# Laços de Repetição 🔁

##### Antes de falar sobre **FOR** ou **WHILE**, vamos entender o que é uma estrutura de repetição.

##### Nas linguagens de programação, existem estruturas para executar um determinado bloco de códigos por uma quantidade de vezes determinada por uma condição (**While**) ou por uma quantidade de vezes (**for**).

##### Agora com uma noção do que é uma estrutura de repetição, vamos começar a falar da estrutura de repetição **FOR**.

##### O **for** em Python é uma estrutura de controle de fluxo que permite iterar sobre uma sequência (como uma lista, tupla, string ou um intervalo de números). Ele executa um bloco de código para cada item da sequência, facilitando a repetição de tarefas de forma eficiente e legível.

#### Sintaxe do for

```python
for i in range(n):
    print(i)
```

##### O **range** é o intervalo em que ele executará o programa.

##### Se o valor de **n** for 10, o nosso range será `(0, 1, 2, 3, 4, 5, 6, 7, 8, 9)`. Opa... ele não vai até o 10? As linguagens de programação sempre começam a contar do 0. Traduzindo para nossa língua, no **for**, ele começa a contar do 0 e vai até o **n – 1**. Ou seja, o **n** não é incluído na sequência.

##### E se eu quiser começar de outro valor? Como faz?

##### Nesse ponto, podemos colocar valores de início e fim no **for**, por exemplo:

```python
for i in range(2, n):
```

##### No exemplo, o **for** vai começar em 2 e ir até o **n – 1**.

##### Dá para colocar “pulos” no for?

##### A resposta é **sim**! Vou te mostrar como ficaria a sintaxe:

```python
for i in range(inicio, fim, pulo):
```

##### Supondo que o **início** seja igual a 2, o **fim** igual a 100 e o **pulo** igual a 5. O programa irá exibir a seguinte ordem: 2, 7, 12, 17,..., 87, 92 e finalizando no 97. Indo de 5 em 5 na repetição.

##### Entendido sobre o **for**, que usamos quando sabemos quantas vezes o programa será repetido, vamos para o **While**, onde não “sabemos” quantas vezes ele será repetido e usamos uma condição para que ele pare.

###### Uma boa prática para usar o **While** é criando uma “bandeira” que inicia a condição verdadeira.
##### Irei explicar com um exemplo
```python
flag = True  # Definimos a flag como verdadeira para iniciar o while
while flag:
    numero = int(input("Digite um número: "))  # Solicita um número ao usuário
    if numero == 0:  # Verifica se o número é igual a 0
        print("Você acertou!")  # Exibe mensagem de acerto
        flag = False  # "Abaixa" a bandeira, encerrando o laço
        break  # Interrompe o laço de repetição
```
##### Vamos entender o que este código faz: no **while** colocamos a nossa flag que tem o valor de True para inicar o laço de repetição, em seguida um input para receber um número para realizar uma comparação.
##### Na condição **if** fazemos uma comparação se o número é igual a um número aleatório que escolhi. Se essa condição for verdadeira, ele entra na condição e escreve que você acertou o número, "baixa" a bandeira e da um break para ENCERRAR o laço de repetição. 
##### Essa **flag** funciona como uma corrida de carros: enquanto a bandeira está verde, os carros continuam dando voltas na pista. Assim que a última volta é alcançada, a bandeira final é levantada, sinalizando que é hora de parar. Nesse código, a bandeira verde representa a condição verdadeira (True) que mantém o laço funcionando. Quando o número certo é digitado, o programa "muda a bandeira" para parar a repetição.
