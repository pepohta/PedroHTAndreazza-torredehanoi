# 03 - Torre de Hanoi (Pilhas)

## Descrição
Este projeto implementa a solução do problema clássico da Torre de Hanói utilizando a estrutura de dados Pilha (stack) e um algoritmo recursivo.

O sistema simula três hastes (A, B e C), onde discos de diferentes tamanhos são movimentados respeitando regras específicas, até transferir todos da haste A para a haste C.

---

## Regras do Problema

- Apenas um disco pode ser movido por vez
- Apenas o disco do topo pode ser movimentado
- Um disco maior nunca pode ficar sobre um menor

---

## Funcionalidades

- Leitura do número de discos (1 a 10)
- Inicialização automática da haste A
- Execução do algoritmo recursivo
- Exibição de cada movimento realizado
- Exibição do estado das hastes a cada passo
- Contagem total de movimentos

---

## Estrutura Utilizada

Foi utilizada a estrutura de dados **Pilha (stack)**.

Cada haste (A, B e C) é representada por uma pilha, onde:

- O topo representa o último disco inserido
- Apenas o topo pode ser removido ou inserido
- Segue o princípio LIFO (Last In, First Out)

---

## Pontos de Análise e Justificativa

### 1. Por que a Pilha é adequada?

A pilha é adequada para este problema porque o acesso aos elementos ocorre apenas pelo topo, o que corresponde às regras da Torre de Hanói.

Como só é permitido mover o disco do topo, a estrutura de pilha é perfeita, garantindo que as operações sejam realizadas de forma correta e controlada.

---

### 2. É possível resolver sem recursão?

Sim, é possível resolver sem recursão utilizando uma abordagem iterativa.

Nesse caso, seria necessário:
- Simular manualmente as chamadas recursivas
- Utilizar pilhas auxiliares para controlar os movimentos
- Implementar lógica adicional para decidir os movimentos

Porém, a recursão é mais adequada porque:
- O problema possui definição naturalmente recursiva
- A solução fica mais simples e direta
- O código fica mais legível

---

## Organização do Projeto

- `include/` → declarações das funções
- `src/` → implementação das funções
- `main.cpp` → execução do programa

---

## Pré-requisitos

- Compilador C++ (GCC/G++)
- Editor de código (VS Code)

---

## Compilação

```bash
- Na pasta /.vscode/:
g++ main.cpp src/hanoi.cpp -o hanoi