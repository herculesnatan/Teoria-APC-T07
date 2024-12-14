# Strings Python
As strings em Python são sequências de caracteres que podem incluir letras, números, símbolos e até espaços. Elas são criadas utilizando aspas simples (‘) ou aspas duplas (“).

### Funções básicas
- `len()` - Retorna o comprimento da string.
- `str.upper()` - Coloca todos os caracteres em letras maiúsculas.
- `str.lower()` - Coloca todos os caracteres em letras minúsculas.
- `str.split()` - Divide uma string em uma lista, usando um delimitador especificado.
- `str.join()` - Junta elementos de uma lista de strings usando um delimitador especificado.
- `str.replace()` - Substitui uma substring por outra string.
- `str.find()` - Retorna o índice da primeira ocorrência de uma substring, ou -1 se não for encontrada.
- `str.count()` - Conta quantas vezes uma substring aparece na string.
- `str.isnumeric()` - Retorna `True` se a string for numérica.
- `str.isalpha()` - Retorna `True` se a string for alfabética.
- `str.isalnum()` - Retorna `True` se a string for alfanumérica.
- `str.isdigit()` - Retorna `True` se a string for um dígito.
- `str.isspace()` - Retorna `True` se a string for um espaço.
- `in` - Retorna `True` se a palavra especificada está presente na string.

### Fatiamento de strings
```python
palavra = "Python"
palavra[0:]  # Começa do índice 0 e vai até o final da string.
palavra[:3]  # Começa do índice 0 e vai até o índice 2 (o 3 é excluído).
palavra[::-1]  # Inverte a string.
palavra[-1]  # Retorna o último caractere da string.
```
O fatiamento ocorre da forma `string[início:fim:pulo]`.

### Tipos de formatação
```python
python
idade = 22
# Forma 1
print(f"Ele tem {idade}")
# Forma 2
print("Ele tem " + str(idade))
# Forma 3
print("Ele tem {}".format(idade))
# Forma 4
print("Ele tem %i" % idade)
```

### Escapes
- `\n` - Nova linha.
- `\t` - Nova tabulação.
- `\\` - Continuação da string em uma nova linha.