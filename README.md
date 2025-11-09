# Guia Completo de Python  
**por DestroyerX**  
## Sumário  
1. Introdução  
2. Estrutura Básica  
3. Variáveis e Tipos de Dados  
4. Operadores  
5. Estruturas Condicionais  
6. Estruturas de Repetição  
7. Funções  
8. Classes e Objetos  
9. Tratamento de Exceções  
10. Manipulação de Arquivos  
11. Módulos e Bibliotecas  
12. Funções Embutidas  
13. Estruturas de Dados - Métodos Úteis  
14. Módulos Importantes  
15. Exemplo Completo  

## Introdução  
Este guia contém **todos os comandos e estruturas mais importantes do Python**, com exemplos práticos e tabelas formatadas para visualização no GitHub Dark Mode.

## Estrutura Básica  
| Comando | Descrição | Exemplo |  
|---------|-----------|---------|  
| `print()` | Exibe mensagem | `print("Olá, mundo!")` |  
| `input()` | Lê entrada | `nome = input("Digite seu nome: ")` |  
| `type()` | Mostra tipo da variável | `type(42)` |  
| `del` | Remove variável ou item | `del x` |  

## Variáveis e Tipos de Dados  
| Tipo | Descrição | Exemplo |  
|------|-----------|---------|  
| `int` | Inteiro | `idade = 25` |  
| `float` | Decimal | `altura = 1.75` |  
| `str` | Texto | `nome = "Ana"` |  
| `bool` | Verdadeiro/Falso | `ativo = True` |  
| `list` | Lista mutável | `frutas = ["maçã","banana"]` |  
| `tuple` | Tupla imutável | `coordenadas = (10,20)` |  
| `dict` | Dicionário | `aluno = {"nome":"João","idade":20}` |  
| `set` | Conjunto | `numeros = {1,2,3}` |  

## Operadores  
| Tipo | Operadores | Exemplo | Resultado |  
|------|-----------|---------|-----------|  
| Aritméticos | `+ - * / // % **` | `2**3` | 8 |  
| Comparação | `== != > < >= <=` | `5!=3` | True |  
| Lógicos | `and or not` | `(5>3) and (2<1)` | False |  
| Atribuição | `= += -= *= /=` | `x+=1` | Soma 1 a x |  
| Pertinência | `in, not in` | `"a" in "casa"` | True |  
| Identidade | `is, is not` | `x is y` | True/False |  
| Bit a bit | `& | ^ << >>` | `5 & 3` | 1 |  

## Estruturas Condicionais  
```python
x = 15
if x > 10:
    print("Maior que 10")
elif x == 10:
    print("Igual a 10")
else:
    print("Menor que 10")
```  

## Estruturas de Repetição  
```python
for i in range(1,6):
    if i == 3:
        continue
    print(i)
```  
| Comando | Descrição |  
|---------|-----------|  
| `for` | Itera sobre sequência |  
| `while` | Repete enquanto verdadeiro |  
| `break` | Interrompe loop |  
| `continue` | Pula para próxima iteração |  
| `pass` | Placeholder, não faz nada |  

## Funções  
```python
def saudacao(nome="Visitante"):
    print(f"Olá, {nome}!")
saudacao("Maria")
```  
| Comando | Descrição |  
|---------|-----------|  
| `def` | Define função |  
| `return` | Retorna valor |  
| `lambda` | Função anônima |  
| `*args` | Argumentos variáveis |  
| `**kwargs` | Argumentos nomeados |  

## Classes e Objetos  
```python
class Pessoa:
    def __init__(self,nome):
        self.nome = nome
    def apresentar(self):
        print(f"Olá, meu nome é {self.nome}")
p1 = Pessoa("João")
p1.apresentar()
```  
| Comando | Descrição |  
|---------|-----------|  
| `class` | Define classe |  
| `__init__` | Construtor |  
| `self` | Referência ao próprio objeto |  
| `method` | Método da classe |  

## Tratamento de Exceções  
```python
try:
    n = int(input("Digite um número: "))
except ValueError:
    print("Número inválido")
finally:
    print("Fim do programa")
```  
| Comando | Descrição |  
|---------|-----------|  
| `try` | Bloco que pode gerar erro |  
| `except` | Trata erro |  
| `else` | Executa se não houver erro |  
| `finally` | Executa sempre |  
| `raise` | Lança exceção |  

## Manipulação de Arquivos  
```python
with open("dados.txt","w") as arquivo:
    arquivo.write("Aprendendo Python!")
```  
| Comando | Descrição |  
|---------|-----------|  
| `open()` | Abrir arquivo |  
| `read()` | Ler conteúdo |  
| `write()` | Escrever conteúdo |  
| `close()` | Fechar arquivo |  
| `with` | Abre e fecha automaticamente |  

## Módulos e Bibliotecas  
```python
import math
from math import sqrt
import numpy as np
```  
| Comando | Descrição |  
|---------|-----------|  
| `import` | Importa módulo |  
| `from ... import ...` | Importa parte específica |  
| `as` | Cria apelido para módulo |  

## Funções Embutidas  
| Função | Descrição | Exemplo | Resultado |  
|--------|-----------|---------|-----------|  
| `len()` | Tamanho | `len("Python")` | 6 |  
| `max()` | Maior valor | `max([1,2,3])` | 3 |  
| `min()` | Menor valor | `min([1,2,3])` | 1 |  
| `sum()` | Soma | `sum([1,2,3])` | 6 |  
| `sorted()` | Ordena | `sorted([3,1,2])` | [1,2,3] |  

## Estruturas de Dados - Métodos Úteis  
| Tipo | Métodos | Exemplo |  
|------|--------|---------|  
| Lista | append(), extend(), remove(), sort(), reverse() | `frutas.append("laranja")` |  
| Dicionário | keys(), values(), items(), get() | `dados.get("nome")` |  
| Conjunto | add(), union(), intersection() | `A.union(B)` |  

## Módulos Importantes  
| Módulo | Uso |  
|--------|-----|  
| math | Funções matemáticas |  
| datetime | Data e hora |  
| os | Sistema operacional |  
| sys | Parâmetros e ambiente |  
| random | Números aleatórios |  
| json | Arquivos JSON |  
| re | Expressões regulares |  
| collections | Estruturas avançadas |  
| itertools | Iteração avançada |  
| functools | Funções de alta ordem |  

## Exemplo Completo  
```python
nomes = []
while True:
    n = input("Digite um nome (ou 'sair'): ")
    if n.lower() == "sair":
        break
    nomes.append(n)

print("\\nNomes cadastrados:")
for nome in sorted(nomes):
    print(nome)
```  

**Fim do Guia Python — por DestroyerX**
