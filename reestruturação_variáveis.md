
# Reatribuição de valores em variáveis

Observe o seguinte caso: você está tentando resolver um problema em que recebe várias entradas e a cada nova entrada precisa analisar se o valor recebido é maior ou não que valor da variável atual. Talvez ainda esteja um pouco confuso tudo isso, mas irei tentar exemplificar melhor.

Imagine que queremos comparar salários inseridos pelo usuário e registrar qual é o seu maior valor até o momento.

```python
# Inicializamos a variável com um valor base
maior_salario = 0

# Recebemos uma entrada de salário (como exemplo)
salario = float(input("Digite o salário: "))
```

Veja que criei e atribuí um valor base à variável `maior_salario`, igual a 0. Bom, agora, ao receber nossa primeira entrada, vamos fazer uma comparação com essa variável.

```python
# Verificamos se o salário recebido é maior que o maior_salario atual
if salario > maior_salario:

    # Atualizamos maior_salario com o novo valor
    maior_salario = salario

print(f"O maior salário registrado até agora é: {maior_salario}")
```

Vamos entender o que foi feito. Primeiro fizemos a comparação se o salário digitado pelo usuário é maior do que o salário declarado inicialmente na variável, se essa condição for verdadeira vamos entrar na seguinte situação: reatribuir o valor de `salario` em `maior_salario`.

Pense em uma variável como algo escrito em um quadro de giz. Quando atualizamos o valor, apagamos o que estava escrito e substituímos pelo novo valor. A reatribuição funciona exatamente dessa forma.
