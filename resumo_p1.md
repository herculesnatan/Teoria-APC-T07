# Resumo P1

## **Variáveis**  
As variáveis são usadas para armazenar valores que podem ser reutilizados ao longo do código.  
- Não é necessário declarar o tipo, pois Python é uma linguagem de tipagem dinâmica.  
Exemplo:  
```python
x = 10  # Inteiro
nome = "João"  # String
pi = 3.14  # Float
boo = True # Boolean
```

## **Expressões**  
Expressões combinam variáveis, valores e operadores para realizar cálculos ou avaliar condições.  
- **Operadores matemáticos**: `+`, `-`, `*`, `/`, `//`, `%`, `**`.  
- **Operadores de comparação**: `==`, `!=`, `<`, `>`, `<=`, `>=`.  
- **Operadores lógicos**: `and`, `or`, `not`.  
Exemplo:  
```python
a = 5
b = 3
resultado = (a + b) * 2  # 16
```

## **Condicionais**  
Os condicionais permitem executar diferentes blocos de código com base em condições.  
- Usam as palavras-chave: `if`, `elif`, `else`.  
Exemplo:  
```python
idade = 18
if idade >= 18:
    print("Maior de idade")
else:
    print("Menor de idade")
```

## **Iteração**  
As estruturas de repetição permitem executar um bloco de código várias vezes.  
- **`for`**: Ideal para iterar sobre sequências (listas, strings, etc.).  
- **`while`**: Continua executando enquanto a condição for verdadeira.  
Exemplos:  
```python
# For
for i in range(5):  # Itera de 0 a 4
    print(i)

# While
contador = 0
while contador < 5:
    print(contador)
    contador += 1
```

## **Funções**  
As funções encapsulam blocos de código reutilizáveis.  
- Definidas com a palavra-chave `def`.  
Exemplo:  
```python
def saudacao(nome):
    return f"Olá, {nome}!"

print(saudacao("Maria"))  # Saída: Olá, Maria!
```

## **Strings**  
As strings representam sequências de caracteres.  
- Podem ser manipuladas com índices, métodos e operadores.  
Exemplo:  
```python
texto = "Python"
print(texto[0])  # P (primeiro caractere)
print(len(texto))  # 6 (tamanho da string)
print(texto.upper())  # PYTHON (em maiúsculas)
print(texto[::-1])  # nohtyP (inverso da string)
print(texto[0:3]) # Pyt
```


## **`split()`**  
A função `split` é usada para dividir uma string em uma lista com base em um delimitador especificado.  
- Por padrão, o delimitador é um espaço em branco.  
- Você pode especificar outro delimitador, como vírgula, ponto, etc.  
- Útil para processar entradas de texto.  

### Exemplo:  
```python
texto = "Python é incrível"
# Dividindo por espaços (padrão)
palavras = texto.split()
print(palavras)  # ['Python', 'é', 'incrível']

# Dividindo por um delimitador específico
data = "01/01/2024"
partes = data.split("/")
print(partes)  # ['01', '01', '2024']
```


## **`map()`**  
A função `map` aplica uma função a todos os elementos de um iterável (como listas ou tuplas).  
- Retorna um objeto do tipo `map`, que pode ser convertido em uma lista, tupla ou outro iterável.  
- Útil para transformar ou processar elementos de uma sequência de forma eficiente.  

### Exemplo:  
```python

# Convertendo uma lista de strings em inteiros
valores = ["10", "20", "30"]
inteiros = map(int, valores)
print(list(inteiros))  # [10, 20, 30]
```

### **Usando `split` e `map` juntos**  
Essas funções são frequentemente combinadas para processar entradas de texto e convertê-las em outro tipo de dado.  

### Exemplo:  
```python
entrada = "1 2 3 4 5"
# Dividir a string em números e convertê-los para inteiros
numeros = list(map(int, entrada.split()))
print(numeros)  # [1, 2, 3, 4, 5]
```

