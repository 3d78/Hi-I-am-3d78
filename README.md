# Guia Completo de Python  
**por DestroyerX**

```python
# Estrutura Básica
print("Olá, mundo!")        # Exibe mensagem
nome = input("Digite seu nome: ")  # Lê entrada
type(42)                    # Mostra tipo da variável
del nome                     # Remove variável
```

```python
# Variáveis e Tipos de Dados
idade = 25           # int
altura = 1.75        # float
nome = "Ana"         # str
ativo = True         # bool
frutas = ["maçã","banana"]  # list
coordenadas = (10,20)       # tuple
aluno = {"nome":"João","idade":20}  # dict
numeros = {1,2,3}             # set
```

```python
# Operadores
a, b = 5, 3
soma = a + b
sub = a - b
mul = a * b
div = a / b
div_int = a // b
mod = a % b
pot = a ** b
print((a > b) and (b < a))  # Operador lógico
```

```python
# Estruturas Condicionais
x = 15
if x > 10:
    print("Maior que 10")
elif x == 10:
    print("Igual a 10")
else:
    print("Menor que 10")
```

```python
# Estruturas de Repetição
for i in range(1,6):
    if i == 3:
        continue
    print(i)

while x > 0:
    print(x)
    x -= 1
```

```python
# Funções
def saudacao(nome="Visitante"):
    print(f"Olá, {nome}!")

saudacao("Maria")

# Função lambda
dobro = lambda x: x*2
print(dobro(5))
```

```python
# Classes e Objetos
class Pessoa:
    def __init__(self, nome):
        self.nome = nome
    def apresentar(self):
        print(f"Olá, meu nome é {self.nome}")

p1 = Pessoa("João")
p1.apresentar()
```

```python
# Tratamento de Exceções
try:
    n = int(input("Digite um número: "))
except ValueError:
    print("Número inválido")
finally:
    print("Fim do programa")
```

```python
# Manipulação de Arquivos
with open("dados.txt", "w") as arquivo:
    arquivo.write("Aprendendo Python!")

with open("dados.txt", "r") as arquivo:
    print(arquivo.read())
```

```python
# Módulos e Bibliotecas
import math
from math import sqrt
import random as r

print(math.pi)
print(sqrt(25))
print(r.randint(1,10))
```

```python
# Estruturas de Dados - Métodos Úteis
frutas.append("laranja")
dados.get("nome")
A.union(B)
```

```python
# Exemplo Completo
nomes = []
while True:
    n = input("Digite um nome (ou 'sair'): ")
    if n.lower() == "sair":
        break
    nomes.append(n)

print("\nNomes cadastrados:")
for nome in sorted(nomes):
    print(nome)
```

**Fim do Guia Python — por DestroyerX**
