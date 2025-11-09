🔹 1. ESTRUTURA BÁSICA DA LINGUAGEM
2. | Comando / Estrutura | Descrição                              | Exemplo                             |
| ------------------- | -------------------------------------- | ----------------------------------- |
| `print()`           | Exibe uma mensagem na tela.            | `print("Olá, mundo!")`              |
| `input()`           | Lê uma entrada do usuário.             | `nome = input("Digite seu nome: ")` |
| `type()`            | Mostra o tipo de dado de uma variável. | `print(type(42))` → `<class 'int'>` |
| `del`               | Remove variáveis, listas, itens etc.   | `del x`                             |

🔹 2. VARIÁVEIS E TIPOS DE DADOS
3. | Tipo    | Descrição                       | Exemplo                                 |
| ------- | ------------------------------- | --------------------------------------- |
| `int`   | Número inteiro                  | `idade = 25`                            |
| `float` | Número decimal                  | `altura = 1.75`                         |
| `str`   | Texto (string)                  | `nome = "Ana"`                          |
| `bool`  | Verdadeiro/Falso                | `ativo = True`                          |
| `list`  | Lista mutável                   | `frutas = ["maçã", "banana", "uva"]`    |
| `tuple` | Tupla imutável                  | `coordenadas = (10, 20)`                |
| `dict`  | Dicionário (pares chave: valor) | `aluno = {"nome": "João", "idade": 20}` |
| `set`   | Conjunto (valores únicos)       | `numeros = {1, 2, 3}`                   |

🔹 3. OPERADORES
| Tipo        | Operadores                          | Exemplo               | Resultado                      |     |
| ----------- | ----------------------------------- | --------------------- | ------------------------------ | --- |
| Aritméticos | `+`, `-`, `*`, `/`, `//`, `%`, `**` | `2 ** 3`              | `8`                            |     |
| Comparação  | `==`, `!=`, `>`, `<`, `>=`, `<=`    | `5 != 3`              | `True`                         |     |
| Lógicos     | `and`, `or`, `not`                  | `(5 > 3) and (2 < 1)` | `False`                        |     |
| Atribuição  | `=`, `+=`, `-=`, `*=`, `/=`, etc.   | `x += 1`              | Soma 1 a `x`                   |     |
| Pertinência | `in`, `not in`                      | `"a" in "casa"`       | `True`                         |     |
| Identidade  | `is`, `is not`                      | `x is y`              | Verifica se são o mesmo objeto |     |
| Bit a bit   | `&`, `                              | `, `^`, `<<`, `>>`    | `5 & 3`                        | `1` |

🔹 4. ESTRUTURAS CONDICIONAIS
| Comando | Descrição                                      | Exemplo                            |
| ------- | ---------------------------------------------- | ---------------------------------- |
| `if`    | Executa um bloco se a condição for verdadeira. | `if x > 10: print("Maior que 10")` |
| `elif`  | Verifica nova condição se a anterior falhar.   | `elif x == 10:`                    |
| `else`  | Executa se todas as condições falharem.        | `else: print("Menor que 10")`      |

🔹 Exemplo pratico:
| ------- | ---------------------------------------------- | ---------------------------------- |
x = 15
if x > 10:
    print("Maior que 10")
elif x == 10:
    print("Igual a 10")
else:
    print("Menor que 10")
| ------- | ---------------------------------------------- | ---------------------------------- |

🔹 5. ESTRUTURAS DE REPETIÇÃO
| Comando    | Descrição                                  | Exemplo                       |
| ---------- | ------------------------------------------ | ----------------------------- |
| `for`      | Itera sobre uma sequência.                 | `for i in range(5): print(i)` |
| `while`    | Repete enquanto a condição for verdadeira. | `while x < 10: x += 1`        |
| `break`    | Interrompe o loop.                         | `if i == 3: break`            |
| `continue` | Pula para a próxima iteração.              | `if i == 2: continue`         |
| `pass`     | Não faz nada (usado como placeholder).     | `if cond: pass`               |

🔹 Exemplo:
| ---------- | ------------------------------------------ | ----------------------------- |
for i in range(1, 6):
    if i == 3:
        continue
    print(i)
| ---------- | ------------------------------------------ | ----------------------------- |

🔹 6. FUNÇÕES
| Comando    | Descrição             | Exemplo                           |
| ---------- | --------------------- | --------------------------------- |
| `def`      | Define uma função.    | `def soma(a, b): return a + b`    |
| `return`   | Retorna um valor.     | `return resultado`                |
| `lambda`   | Cria função anônima.  | `dobro = lambda x: x*2`           |
| `*args`    | Argumentos variáveis. | `def soma(*n): return sum(n)`     |
| `**kwargs` | Argumentos nomeados.  | `def info(**dados): print(dados)` |

🔹 Exemplo:
| ---------- | ------------------------------------------ | ----------------------------- |
def saudacao(nome="Visitante"):
    print(f"Olá, {nome}!")

saudacao("Maria")
| ---------- | ------------------------------------------ | ----------------------------- |

🔹 7. CLASSES E OBJETOS (POO)
| Comando    | Descrição                     | Exemplo                     |
| ---------- | ----------------------------- | --------------------------- |
| `class`    | Define uma classe.            | `class Pessoa:`             |
| `__init__` | Construtor da classe.         | `def __init__(self, nome):` |
| `self`     | Referência ao próprio objeto. | `self.nome = nome`          |
| `method`   | Define métodos da classe.     | `def falar(self): ...`      |

🔹 Exemplo:
| ---------- | ----------------------------- | --------------------------- |
class Pessoa:
    def __init__(self, nome):
        self.nome = nome

    def apresentar(self):
        print(f"Olá, meu nome é {self.nome}")

p1 = Pessoa("João")
p1.apresentar()
| ---------- | ----------------------------- | --------------------------- |

🔹 8. TRATAMENTO DE EXCEÇÕES
| Comando   | Descrição                             | Exemplo                     |
| --------- | ------------------------------------- | --------------------------- |
| `try`     | Bloco com código que pode gerar erro. | `try: x = 1 / 0`            |
| `except`  | Trata o erro.                         | `except ZeroDivisionError:` |
| `else`    | Executa se não houver erro.           | `else: print("Sem erro")`   |
| `finally` | Executa sempre.                       | `finally: print("Fim")`     |
| `raise`   | Lança um erro.                        | `raise ValueError("Erro!")` |

🔹 Exemplo:
| ---------- | ----------------------------- | --------------------------- |
try:
    n = int(input("Digite um número: "))
except ValueError:
    print("Por favor, insira um número válido.")
finally:
    print("Fim do programa.")
| ---------- | ----------------------------- | --------------------------- |

🔹 9. MANIPULAÇÃO DE ARQUIVOS
| Comando   | Descrição                     | Exemplo                        |
| --------- | ----------------------------- | ------------------------------ |
| `open()`  | Abre um arquivo.              | `f = open("arquivo.txt", "r")` |
| `read()`  | Lê conteúdo.                  | `conteudo = f.read()`          |
| `write()` | Escreve conteúdo.             | `f.write("Olá")`               |
| `close()` | Fecha o arquivo.              | `f.close()`                    |
| `with`    | Abre e fecha automaticamente. | `with open("a.txt") as f:`     |

🔹 Exemplo:
| --------- | ----------------------------- | ------------------------------ |
with open("dados.txt", "w") as arquivo:
    arquivo.write("Aprendendo Python!")
| --------- | ----------------------------- | ------------------------------ |

Guia_Completo_Python_by_DestroyerX.md





