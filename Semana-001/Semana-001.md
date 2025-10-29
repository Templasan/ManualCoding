#  LISTA SEMANA-001

> Entregar em código e escrever no papel

<details>
<summary>Exercício 01 — Soma de Elementos de uma Lista</summary>

**Tema:** Array – Manipulação Básica  
**Dificuldade:** Fácil  

### Enunciado
Crie uma função em Python chamada `soma_lista` que receba uma lista de números inteiros e retorne a soma de todos os elementos da lista.  

**Exemplo de entrada e saída:**
```
entrada = [1, 2, 3, 4, 5]
saida = soma_lista(entrada)
print(saida)  # 15
```

### Requisitos / Limitações
Não utilize a função built-in sum().

Percorra a lista usando loops (for ou while).

A função deve retornar 0 caso a lista esteja vazia.

Dica: inicialize uma variável acumuladora e vá somando os elementos da lista.

</details>

---

<details>
<summary>Exercício 02 — Soma de Subarrays (Prefix Sum)</summary>

**Tema:** Array – Prefix Sum  
**Dificuldade:** Fácil  

### Enunciado
Crie uma função em Python chamada `prefix_sum` que receba uma lista de números inteiros `nums` e um inteiro `k`, e retorne uma lista contendo a soma de todos os subarrays de tamanho `k`.

**Exemplo de entrada e saída:**
```
nums = [1, 2, 3, 4, 5]
k = 3
saida = prefix_sum(nums, k)
print(saida) # [6, 9, 12]
```

**Explicação:**  
```
- Subarray [1, 2, 3] → soma = 6  
- Subarray [2, 3, 4] → soma = 9  
- Subarray [3, 4, 5] → soma = 12  

```

### Requisitos / Limitações
Não utilize funções externas como numpy.sum().

Use Prefix Sum ou Sliding Window para otimizar a solução.

Caso `k` seja maior que o tamanho da lista, retorne uma lista vazia.

Dica: calcule a soma inicial do primeiro subarray e depois atualize somando o próximo elemento e subtraindo o primeiro do subarray anterior.

</details>

---

<details>
<summary>Exercício 03 — Verificar Palíndromo</summary>

**Tema:** Strings  
**Dificuldade:** Fácil  

### Enunciado
Crie uma função em Python chamada `eh_palindromo` que receba uma string `s` e retorne `True` se a string for um palíndromo, ou `False` caso contrário.  

**Exemplo de entrada e saída:**
```

entrada = "arara"
saida = eh_palindromo(entrada)
print(saida)  # True

entrada = "python"
saida = eh_palindromo(entrada)
print(saida)  # False

```

### Requisitos / Limitações
Não utilize bibliotecas externas.

Considere apenas os caracteres alfabéticos e ignore maiúsculas/minúsculas.

Dica: você pode comparar a string com sua versão invertida.

</details>

---

<details>
<summary>Exercício 04 — Verificar Anagramas</summary>

**Tema:** Strings  
**Dificuldade:** Fácil  

### Enunciado
Crie uma função em Python chamada `sao_anagramas` que receba duas strings `s1` e `s2` e retorne `True` se elas forem anagramas, ou `False` caso contrário.  

**Exemplo de entrada e saída:**
```

s1 = "roma"
s2 = "amor"
saida = sao_anagramas(s1, s2)
print(saida)  # True

s1 = "python"
s2 = "typhon"
saida = sao_anagramas(s1, s2)
print(saida)  # True

s1 = "python"
s2 = "java"
saida = sao_anagramas(s1, s2)
print(saida)  # False

```

### Requisitos / Limitações
Não utilize bibliotecas externas.

Considere que a comparação deve ignorar maiúsculas/minúsculas.

Dica: você pode usar `dict` ou `Counter` para contar a frequência de cada caractere.

</details>

---

<details>
<summary>Exercício 05 — Frequência de Caracteres</summary>

**Tema:** Hash Map / Dicionários  
**Dificuldade:** Fácil  

### Enunciado
Crie uma função em Python chamada `frequencia_caracteres` que receba uma string `s` e retorne um dicionário contendo a contagem de cada caractere presente na string.  

**Exemplo de entrada e saída:**
```

entrada = "banana"
saida = frequencia_caracteres(entrada)
print(saida)  # {'b': 1, 'a': 3, 'n': 2}

```

### Requisitos / Limitações
Não utilize bibliotecas externas.

Considere apenas caracteres alfabéticos e ignore maiúsculas/minúsculas.

Dica: percorra a string e atualize a contagem em um dicionário.

</details>

---

<details>
<summary>Exercício 06 — Two Sum</summary>

**Tema:** Hash Map / Dicionários  
**Dificuldade:** Fácil  

### Enunciado
Crie uma função em Python chamada `two_sum` que receba uma lista de números inteiros `nums` e um inteiro `target`.  
A função deve retornar uma tupla com os índices de dois números distintos que somam exatamente `target`. Se não houver solução, retorne `None`.  

**Exemplo de entrada e saída:**
```

nums = [2, 7, 11, 15]
target = 9
saida = two_sum(nums, target)
print(saida)  # (0, 1)

```

### Requisitos / Limitações
Não utilize loops duplos para verificar todos os pares (O(N²)).

Use um dicionário para armazenar os números já vistos e otimizar a busca (O(N)).

Dica: para cada número `n`, verifique se `target - n` já está no dicionário.

</details>

---

<details>
<summary>Exercício 07 — Par Ordenado (Two Pointers)</summary>

**Tema:** Two Pointers  
**Dificuldade:** Fácil  

### Enunciado
Crie uma função em Python chamada `par_ordenado` que receba uma lista de números inteiros **ordenada** `nums` e um inteiro `target`.  
A função deve retornar `True` se existir um par de elementos distintos na lista que some exatamente `target`, ou `False` caso contrário.  

**Exemplo de entrada e saída:**
```

nums = [1, 2, 4, 5, 7, 11]
target = 9
saida = par_ordenado(nums, target)
print(saida)  # True  (2 + 7)

nums = [1, 3, 5, 6]
target = 10
saida = par_ordenado(nums, target)
print(saida)  # False

```

### Requisitos / Limitações
Não utilize loops duplos para checar todos os pares (O(N²)).

Use a técnica de **dois ponteiros** para percorrer a lista de forma eficiente (O(N)).

Dica: inicialize um ponteiro no início e outro no fim da lista, e mova-os dependendo da soma atual.

</details>

---

<details>
<summary>Exercício 08 — Linked List: Inserção e Remoção</summary>

**Tema:** Linked Lists  
**Dificuldade:** Fácil  

### Enunciado
Crie uma classe em Python chamada `Node` representando um nó de uma linked list, e uma classe `LinkedList` que suporte inserção no final e remoção de um elemento específico pelo valor.  

**Exemplo de uso:**
```

lista = LinkedList()
lista.inserir(1)
lista.inserir(2)
lista.inserir(3)
lista.remover(2)

# A lista agora contém: 1 -> 3

lista.imprimir()  # 1 -> 3

```

### Requisitos / Limitações
- Implemente sua própria linked list (não use listas Python para simular a estrutura).
- A função `remover` deve lidar corretamente com elementos que não existem na lista.
- A função `imprimir` deve exibir todos os elementos da lista em ordem.

Dica: use um nó "dummy" (sentinela) para simplificar remoções no início da lista.

</details>

---

<details>
<summary>Exercício 09 — Parênteses Balanceados</summary>

**Tema:** Stacks  
**Dificuldade:** Fácil  

### Enunciado
Crie uma função em Python chamada `parenteses_balanceados` que receba uma string contendo apenas os caracteres `'('`, `')'`, `'{'`, `'}'`, `'['` e `']'`.  
A função deve retornar `True` se todos os parênteses estiverem balanceados e fechando na ordem correta, ou `False` caso contrário.  

**Exemplo de entrada e saída:**
```

entrada = "([{}])"
saida = parenteses_balanceados(entrada)
print(saida)  # True

entrada = "([)]"
saida = parenteses_balanceados(entrada)
print(saida)  # False

```

### Requisitos / Limitações
- Use uma **stack** (`list` ou `collections.deque`) para auxiliar na verificação.
- Não utilize bibliotecas externas.

Dica: empilhe os parênteses de abertura e, ao encontrar um fechamento, verifique se corresponde ao topo da stack.

</details>

---

<details>
<summary>Exercício 10 — Simulação de Fila</summary>

**Tema:** Queues  
**Dificuldade:** Fácil  

### Enunciado
Crie uma classe em Python chamada `Fila` que utilize `collections.deque` para simular uma fila (FIFO).  
A classe deve ter os métodos `enfileirar(item)` para adicionar elementos, `desenfileirar()` para remover o elemento da frente, e `esta_vazia()` para verificar se a fila está vazia.  

**Exemplo de uso:**
```

fila = Fila()
fila.enfileirar(1)
fila.enfileirar(2)
fila.enfileirar(3)
print(fila.desenfileirar())  # 1
print(fila.esta_vazia())     # False

```

### Requisitos / Limitações
- Utilize `collections.deque` para a implementação.
- A função `desenfileirar` deve retornar `None` se a fila estiver vazia.

Dica: a fila deve seguir a ordem **FIFO** (primeiro a entrar, primeiro a sair).

</details>

---

<details>
<summary>Exercício 11 — Sliding Window: Soma Máxima</summary>

**Tema:** Array – Sliding Window  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `soma_maxima_janela` que receba uma lista de números inteiros `nums` e um inteiro `k` representando o tamanho da janela.  
A função deve retornar a **soma máxima** de `k` elementos consecutivos na lista.  

**Exemplo de entrada e saída:**
```

nums = [2, 1, 5, 1, 3, 2]
k = 3
saida = soma_maxima_janela(nums, k)
print(saida)  # 9  (5 + 1 + 3)

```

### Requisitos / Limitações
- Utilize a técnica de **sliding window** para otimizar a solução (O(N)).
- Não use loops aninhados para somar todas as janelas possíveis.

Dica: inicialize a soma da primeira janela e depois deslize a janela adicionando o novo elemento e subtraindo o que saiu.

</details>

---

<details>
<summary>Exercício 12 — Substring Mais Longa sem Repetição</summary>

**Tema:** Strings – Sliding Window  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `substring_unica` que receba uma string `s` e retorne o comprimento da **substring mais longa** que não contém caracteres repetidos.  

**Exemplo de entrada e saída:**
```

entrada = "abcabcbb"
saida = substring_unica(entrada)
print(saida)  # 3  ("abc")

entrada = "bbbbb"
saida = substring_unica(entrada)
print(saida)  # 1  ("b")

```

### Requisitos / Limitações
- Utilize a técnica de **sliding window** para otimizar a solução.
- Não use bibliotecas externas.

Dica: use um dicionário ou set para rastrear os caracteres presentes na janela atual e ajuste o início da janela conforme necessário.

</details>

---

<details>
<summary>Exercício 13 — Detectar Elementos Duplicados</summary>

**Tema:** Hash Map / Set  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `tem_duplicados` que receba uma lista de números inteiros `nums` e retorne `True` se houver **elementos duplicados**, ou `False` caso contrário.  

**Exemplo de entrada e saída:**
```

nums = [1, 2, 3, 4, 5]
print(tem_duplicados(nums))  # False

nums = [1, 2, 3, 2]
print(tem_duplicados(nums))  # True

```

### Requisitos / Limitações
- Utilize **sets** ou **dicionários** para detectar duplicatas de forma eficiente (O(N)).
- Não utilize loops duplos (O(N²)).

Dica: percorra a lista e verifique se o elemento já foi visto anteriormente.

</details>

---

<details>
<summary>Exercício 14 — Remover Duplicatas de Lista Ordenada</summary>

**Tema:** Two Pointers  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `remover_duplicatas` que receba uma **lista ordenada** de números inteiros `nums` e remova as duplicatas **in-place**, retornando o novo comprimento da lista sem duplicatas.  

**Exemplo de entrada e saída:**
```

nums = [1, 1, 2, 2, 3]
novo_tamanho = remover_duplicatas(nums)
print(novo_tamanho)  # 3
print(nums[:novo_tamanho])  # [1, 2, 3]

```

### Requisitos / Limitações
- Utilize a técnica de **dois ponteiros** para resolver o problema em O(N).
- Não use listas auxiliares ou funções prontas como `set`.

Dica: mantenha um ponteiro de escrita para sobrescrever duplicatas e outro ponteiro de leitura para percorrer a lista.

</details>

---

<details>
<summary>Exercício 15 — Inversão de Linked List</summary>

**Tema:** Linked List – Inversão  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `inverter_linked_list` que receba a **cabeça** de uma linked list e retorne a **nova cabeça** da lista invertida.  

**Exemplo de uso:**
```

# Estrutura do nó

class Node:
def **init**(self, val):
self.val = val
self.next = None

# Lista: 1 -> 2 -> 3 -> None

head = Node(1)
head.next = Node(2)
head.next.next = Node(3)

nova_cabeca = inverter_linked_list(head)

# Lista invertida: 3 -> 2 -> 1 -> None

```

### Requisitos / Limitações
- Inverter a linked list **in-place**, sem criar novos nós.
- Use **ponteiros** para manipular a referência dos nós.

Dica: percorra a lista e altere o `next` de cada nó para apontar para o nó anterior.

</details>

---

<details>
<summary>Exercício 16 — Soma de Lista Recursiva</summary>

**Tema:** Recursão – Básica  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `soma_lista_recursiva` que receba uma lista de números inteiros `nums` e retorne a soma de todos os elementos **usando recursão**.  

**Exemplo de entrada e saída:**
```

entrada = [1, 2, 3, 4, 5]
saida = soma_lista_recursiva(entrada)
print(saida)  # 15

```

### Requisitos / Limitações
- Não utilize loops (`for` ou `while`) nem a função `sum()`.
- Use recursão para somar os elementos da lista.
- A função deve retornar 0 caso a lista esteja vazia.

Dica: defina um **caso base** para uma lista vazia ou com um elemento, e depois faça a soma do primeiro elemento com a soma recursiva do restante da lista.

</details>

---

<details>
<summary>Exercício 17 — Fibonacci Recursivo</summary>

**Tema:** Recursão – Básica  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `fibonacci` que receba um inteiro `n` e retorne o **n-ésimo termo** da sequência de Fibonacci, utilizando **recursão**.  

**Exemplo de entrada e saída:**
```

print(fibonacci(0))  # 0
print(fibonacci(1))  # 1
print(fibonacci(6))  # 8  (0, 1, 1, 2, 3, 5, 8)

```

### Requisitos / Limitações
- Não utilize loops nem listas auxiliares.
- Utilize recursão pura para calcular o termo.
- Considere que `fibonacci(0) = 0` e `fibonacci(1) = 1`.

Dica: defina **casos base** para `n = 0` e `n = 1`, e o caso recursivo como `fibonacci(n-1) + fibonacci(n-2)`.

</details>

---

<details>
<summary>Exercício 18 — Verificar Número Primo</summary>

**Tema:** Math & Geometry – Básico  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `eh_primo` que receba um número inteiro `n` e retorne `True` se `n` for primo, ou `False` caso contrário.  

**Exemplo de entrada e saída:**
```

print(eh_primo(2))   # True
print(eh_primo(15))  # False
print(eh_primo(17))  # True

```

### Requisitos / Limitações
- Não utilize bibliotecas externas como `math`.
- Utilize apenas loops e operações básicas.
- Considere que números menores que 2 não são primos.

Dica: verifique se `n` é divisível por algum número de 2 até a raiz quadrada de `n`.

</details>

---

<details>
<summary>Exercício 19 — Contar Bits</summary>

**Tema:** Bit Manipulation  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `contar_bits` que receba um número inteiro `n` e retorne o **número de 1s** na representação binária de `n`.  

**Exemplo de entrada e saída:**
```

print(contar_bits(5))  # 2  (5 em binário: 101)
print(contar_bits(15)) # 4  (15 em binário: 1111)

```

### Requisitos / Limitações
- Não utilize a função `bin()` nem strings para contar os bits.
- Utilize operações bit a bit (`AND`, `SHIFT`) para contar os 1s.
- O número de entrada será sempre não-negativo.

Dica: use a técnica de **Brian Kernighan**, subtraindo 1 e fazendo AND com o número repetidamente até zerar.

</details>

---

<details>
<summary>Exercício 20 — Avaliar Expressão Pós-fixa</summary>

**Tema:** Stack  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `avaliar_posfixa` que receba uma **expressão matemática em notação pós-fixa** (lista de strings) e retorne o resultado da avaliação.  

**Exemplo de entrada e saída:**
```

expressao = ["2", "3", "1", "*", "+", "9", "-"]  # Equivale a 2 + 3*1 - 9
resultado = avaliar_posfixa(expressao)
print(resultado)  # -4

```

### Requisitos / Limitações
- Utilize **uma pilha** (`list` ou `collections.deque`) para avaliar a expressão.
- Suporte apenas operadores: `+`, `-`, `*`, `/`.
- Não use `eval()` ou funções externas.

Dica: percorra a expressão, empilhando números e aplicando o operador nos dois últimos números da pilha quando encontrar um operador.

</details>

---

<details>
<summary>Exercício 21 — Subarray Máximo com Janela Variável</summary>

**Tema:** Array – Sliding Window (Variável)  
**Dificuldade:** Difícil  

### Enunciado
Crie uma função em Python chamada `subarray_max_soma` que receba uma lista de números inteiros `nums` e um inteiro `k` e retorne a **soma máxima de qualquer subarray de tamanho variável até k**.  

**Exemplo de entrada e saída:**
```

nums = [2, 1, 5, 1, 3, 2]
k = 3
resultado = subarray_max_soma(nums, k)
print(resultado)  # 9  (subarray [5,1,3])

```

### Requisitos / Limitações
- A solução deve utilizar a técnica de **Sliding Window com tamanho variável**.
- Não utilize funções built-in de agregação como `sum()` dentro de loops.
- A função deve retornar 0 se a lista estiver vazia ou `k` for 0.

Dica: mantenha uma **janela deslizante** e vá atualizando a soma enquanto ajusta o tamanho da janela.

</details>

---

<details>
<summary>Exercício 22 — Mapear Pares para Two Sum</summary>

**Tema:** Hash Map – Dois Somatórios  
**Dificuldade:** Difícil  

### Enunciado
Crie uma função em Python chamada `two_sum_indices` que receba uma lista de números inteiros `nums` e um alvo `target`. A função deve retornar uma lista de **pares de índices** `(i, j)` distintos tais que `nums[i] + nums[j] == target`.  

**Exemplo de entrada e saída:**
```

nums = [2, 7, 11, 15]
target = 9
resultado = two_sum_indices(nums, target)
print(resultado)  # [(0,1)]

```

### Requisitos / Limitações
- Cada par de índices deve ser único, não repetindo combinações invertidas.
- Utilize **dicionário (hash map)** para otimizar a busca.
- Não use nested loops simples $O(N^2)$.

Dica: percorra a lista, armazenando os números já vistos em um dicionário e verificando se o complemento (target - num) já existe.

</details>

---

<details>
<summary>Exercício 23 — Gerar Todos os Subconjuntos</summary>

**Tema:** Recursão / Backtracking  
**Dificuldade:** Difícil  

### Enunciado
Crie uma função em Python chamada `gerar_subconjuntos` que receba uma lista de números inteiros `nums` e retorne **uma lista com todos os subconjuntos possíveis**.  

**Exemplo de entrada e saída:**
```

nums = [1,2,3]
resultado = gerar_subconjuntos(nums)
print(resultado)

# [[], [1], [2], [3], [1,2], [1,3], [2,3], [1,2,3]]

```

### Requisitos / Limitações
- Utilize **recursão ou backtracking** para gerar os subconjuntos.
- Não use funções built-in como `itertools.combinations`.
- A ordem dos subconjuntos na lista final não importa.

Dica: crie uma função auxiliar que construa os subconjuntos **adicionando ou não cada elemento** recursivamente.

</details>

---

<details>
<summary>Exercício 24 — Distância de Edição</summary>

**Tema:** Strings – Programação Dinâmica  
**Dificuldade:** Difícil  

### Enunciado
Crie uma função em Python chamada `distancia_edicao` que receba duas strings `s1` e `s2` e retorne a **distância mínima de edição** entre elas, considerando as operações: inserção, remoção e substituição de um caractere.  

**Exemplo de entrada e saída:**
```

s1 = "kitten"
s2 = "sitting"
resultado = distancia_edicao(s1, s2)
print(resultado)  # 3

```

### Requisitos / Limitações
- Utilize **programação dinâmica (DP)** para resolver o problema.
- Não utilize funções externas ou módulos que implementem a distância de edição.
- Strings de entrada serão curtas (até 20 caracteres) para facilitar o teste.

Dica: crie uma **tabela 2D** onde `dp[i][j]` representa a distância mínima para os prefixos `s1[:i]` e `s2[:j]`.

</details>

---

<details>
<summary>Exercício 25 — Contar Ilhas em Matrizes</summary>

**Tema:** Queue / BFS  
**Dificuldade:** Difícil  

### Enunciado
Crie uma função em Python chamada `contar_ilhas` que receba uma matriz 2D de 0s e 1s (`grid`) e retorne o **número de áreas conectadas de 1s** (ilhas). A conexão é considerada nas **4 direções** (cima, baixo, esquerda, direita).  

**Exemplo de entrada e saída:**
```

grid = [
[1,1,0,0,0],
[1,1,0,0,0],
[0,0,1,0,0],
[0,0,0,1,1]
]
resultado = contar_ilhas(grid)
print(resultado)  # 3

```

### Requisitos / Limitações
- Utilize **BFS** com **fila (`collections.deque`)** para percorrer a matriz.
- Modifique a matriz original ou use uma matriz de visitados para evitar contar células repetidas.
- Não use DFS recursivo.

Dica: percorra cada célula da matriz; quando encontrar um 1 não visitado, faça BFS para marcar toda a ilha.

</details>

---

<details>
<summary>Exercício 26 — Contar Vogais e Consoantes</summary>

**Tema:** Strings – Manipulação de Caracteres  
**Dificuldade:** Fácil  

### Enunciado
Crie uma função em Python chamada `contar_vogais_consoantes` que receba uma string `texto` e retorne **uma tupla** `(num_vogais, num_consoantes)` representando a quantidade de vogais e consoantes na string.  

**Exemplo de entrada e saída:**
```

texto = "Hello World"
resultado = contar_vogais_consoantes(texto)
print(resultado)  # (3, 7)

```

### Requisitos / Limitações
- Considere apenas letras do alfabeto; ignore números e símbolos.
- A contagem deve ser **case-insensitive**.
- Não use bibliotecas externas.

Dica: defina listas ou conjuntos de vogais e verifique cada caractere da string.

</details>

---

<details>
<summary>Exercício 27 — Verificar Palíndromo</summary>

**Tema:** Strings – Palíndromo  
**Dificuldade:** Fácil  

### Enunciado
Crie uma função em Python chamada `eh_palindromo` que receba uma string `texto` e retorne **True** se a string for um palíndromo e **False** caso contrário.  

**Exemplo de entrada e saída:**
```

texto = "arara"
resultado = eh_palindromo(texto)
print(resultado)  # True

texto = "python"
resultado = eh_palindromo(texto)
print(resultado)  # False

```

### Requisitos / Limitações
- Ignore **diferenças de maiúsculas/minúsculas**.
- Ignore **espaços e caracteres especiais**.
- Não use funções externas para verificação de palíndromo.

Dica: compare a string com sua versão invertida após normalização.

</details>

---

<details>
<summary>Exercício 28 — Verificar Anagramas</summary>

**Tema:** Strings – Anagramas  
**Dificuldade:** Fácil  

### Enunciado
Crie uma função em Python chamada `sao_anagramas` que receba duas strings `s1` e `s2` e retorne **True** se elas forem anagramas e **False** caso contrário.  

**Exemplo de entrada e saída:**
```

s1 = "roma"
s2 = "amor"
resultado = sao_anagramas(s1, s2)
print(resultado)  # True

s1 = "python"
s2 = "typhon"
resultado = sao_anagramas(s1, s2)
print(resultado)  # True

s1 = "teste"
s2 = "tseta"
resultado = sao_anagramas(s1, s2)
print(resultado)  # False

```

### Requisitos / Limitações
- Considere apenas letras e ignore maiúsculas/minúsculas.
- Não use funções externas específicas para anagramas.
- Pode usar `dict` ou `Counter` para contar ocorrências.

Dica: conte a frequência de cada caractere em ambas as strings e compare.

</details>

---

<details>
<summary>Exercício 29 — Substring Mais Longa Sem Repetição</summary>

**Tema:** Strings – Substrings Únicas  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `maior_substring_unica` que receba uma string `texto` e retorne o **comprimento da maior substring** que não possui caracteres repetidos.  

**Exemplo de entrada e saída:**
```

texto = "abcabcbb"
resultado = maior_substring_unica(texto)
print(resultado)  # 3 ("abc")

texto = "bbbbb"
resultado = maior_substring_unica(texto)
print(resultado)  # 1 ("b")

texto = "pwwkew"
resultado = maior_substring_unica(texto)
print(resultado)  # 3 ("wke")

```

### Requisitos / Limitações
- A solução deve ter complexidade **O(n)**.
- Utilize a técnica de **Sliding Window** com HashMap ou Set.
- Não use bibliotecas externas além de estruturas básicas (`set`, `dict`).

</details>

---

<details>
<summary>Exercício 30 — Contar Caracteres Únicos</summary>

**Tema:** Strings – Manipulação de Caracteres  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `contar_unicos` que receba uma string `texto` e retorne a quantidade de caracteres que aparecem **apenas uma vez**.  

**Exemplo de entrada e saída:**
```

texto = "abracadabra"
resultado = contar_unicos(texto)
print(resultado)  # 2 ("c" e "d")

texto = "hello"
resultado = contar_unicos(texto)
print(resultado)  # 2 ("h" e "e")

```

### Requisitos / Limitações
- Ignore maiúsculas/minúsculas.
- Considere apenas letras do alfabeto.
- Pode usar `dict` ou `Counter` para contar ocorrências.
- Não utilize funções externas que retornem diretamente os caracteres únicos.

</details>

---

<details>
<summary>Exercício 31 — Reverter Palavras na Frase</summary>

**Tema:** Strings – Manipulação de Strings  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `reverter_palavras` que receba uma string `frase` e retorne a frase com a **ordem das palavras invertida**, mantendo as letras de cada palavra na mesma ordem.  

**Exemplo de entrada e saída:**
```

frase = "Python é divertido"
resultado = reverter_palavras(frase)
print(resultado)  # "divertido é Python"

frase = "Aprender a programar"
resultado = reverter_palavras(frase)
print(resultado)  # "programar a Aprender"

```

### Requisitos / Limitações
- Preserve os espaços entre as palavras.
- Não inverta os caracteres dentro das palavras.
- Não use bibliotecas externas, apenas métodos de strings nativos.

</details>

---

<details>
<summary>Exercício 32 — Compressão de String Simples</summary>

**Tema:** Strings – Manipulação de Strings  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `compressao_string` que receba uma string `texto` e retorne sua versão **compactada**, onde caracteres consecutivos repetidos são substituídos pelo caractere seguido do número de ocorrências.  

**Exemplo de entrada e saída:**
```

texto = "aaabbc"
resultado = compressao_string(texto)
print(resultado)  # "a3b2c1"

texto = "abcd"
resultado = compressao_string(texto)
print(resultado)  # "a1b1c1d1"

```

### Requisitos / Limitações
- A entrada conterá apenas letras minúsculas.
- Não use bibliotecas externas.
- Percorra a string usando loops e condicional.

</details>

---

<details>
<summary>Exercício 33 — Palíndromos Parciais</summary>

**Tema:** Strings – Palíndromos  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `existe_palindromo` que receba uma string `texto` e retorne `True` se **alguma substring de tamanho ≥ 2** for um palíndromo, e `False` caso contrário.  

**Exemplo de entrada e saída:**
```

texto = "abac"
resultado = existe_palindromo(texto)
print(resultado)  # True ("aba")

texto = "xyz"
resultado = existe_palindromo(texto)
print(resultado)  # False

```

### Requisitos / Limitações
- Substrings de tamanho 1 não são consideradas.
- O algoritmo deve percorrer todas as substrings possíveis.
- Não use bibliotecas externas, apenas recursos nativos de strings.

</details>

---

<details>
<summary>Exercício 34 — Anagramas por Grupo</summary>

**Tema:** Strings – Anagramas  
**Dificuldade:** Médio  

### Enunciado
Crie uma função em Python chamada `agrupar_anagramas` que receba uma lista de strings `palavras` e retorne uma lista de listas, onde cada sublista contém palavras que são **anagramas** entre si.  

**Exemplo de entrada e saída:**
```

palavras = ["bat", "tab", "tap", "pat", "cat"]
resultado = agrupar_anagramas(palavras)
print(resultado)

# [["bat", "tab"], ["tap", "pat"], ["cat"]]

```

### Requisitos / Limitações
- As palavras só contêm letras minúsculas.
- Palavras que não possuem anagramas devem formar uma lista individual.
- Pode usar `dict` ou `defaultdict` para agrupar.
- Não use bibliotecas externas específicas de anagramas.

</details>

---

<details>
<summary>Exercício 35 — Substring Anagramática</summary>

**Tema:** Strings – Anagramas  
**Dificuldade:** Difícil  

### Enunciado
Crie uma função em Python chamada `substrings_anagramas` que receba duas strings `texto` e `padrao` e retorne uma lista com todas as **substrings de `texto` que são anagramas de `padrao`**.  

**Exemplo de entrada e saída:**
```

texto = "cbaebabacd"
padrao = "abc"
resultado = substrings_anagramas(texto, padrao)
print(resultado)

# ["cba", "bac"]

```

### Requisitos / Limitações
- A função deve ser eficiente, evitando verificar todas as combinações explicitamente (use contagem de caracteres ou sliding window).  
- `texto` e `padrao` contêm apenas letras minúsculas.  
- Não use bibliotecas externas, apenas recursos nativos de Python.  

</details>

---

<details>
<summary>Exercício 36 — Palíndromo com Mínimo de Alterações</summary>

**Tema:** Strings – Palíndromos / DP  
**Dificuldade:** Difícil  

### Enunciado
Crie uma função em Python chamada `min_alteracoes_palindromo` que receba uma string `texto` e retorne o **número mínimo de alterações de caracteres** necessárias para transformar `texto` em um palíndromo.  

**Exemplo de entrada e saída:**
```

texto = "abcda"
resultado = min_alteracoes_palindromo(texto)
print(resultado)  # 2  ("abcba" ou "adcda")

```

### Requisitos / Limitações
- Apenas substituições de caracteres são permitidas (não inserir nem remover).  
- Utilize programação dinâmica para otimizar a solução.  
- Não use bibliotecas externas.

</details>

---

<details>
<summary>Exercício 37 — Longest Common Subsequence (LCS)</summary>

**Tema:** Strings – DP  
**Dificuldade:** Difícil  

### Enunciado
Crie uma função em Python chamada `lcs` que receba duas strings `s1` e `s2` e retorne o **tamanho da maior subsequência comum (LCS)** entre elas.  

**Exemplo de entrada e saída:**
```

s1 = "abcde"
s2 = "ace"
resultado = lcs(s1, s2)
print(resultado)  # 3  ("ace")

```

### Requisitos / Limitações
- Utilize programação dinâmica (memoização ou tabulação) para eficiência.  
- Não use bibliotecas externas.  
- Subsequência não precisa ser contígua.  

</details>
