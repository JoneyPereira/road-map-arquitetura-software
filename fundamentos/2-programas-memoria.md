# Como os programas rodam na memória?

## Conceitos Fundamentais

### 1. Gerenciamento de Memória
- **Stack (Pilha)**
  - Armazenamento de variáveis locais
  - LIFO (Last In, First Out)
  - Memória de acesso rápido e tamanho limitado
- **Heap (Monte)**
  - Alocação dinâmica de memória
  - Memória de maior capacidade
  - Gerenciamento mais complexo
- **Segmentos de Memória**
  - Código (Text)
  - Dados (Data)
  - BSS (variáveis não inicializadas)
  - Stack
  - Heap

### 2. Ciclo de Vida de um Programa
1. Carregamento do programa
2. Alocação de memória
3. Execução
4. Liberação de recursos

### 3. Virtual Memory
- Paginação
- Swap
- Memory Mapping

## Problemas Comuns
- Memory Leaks
- Stack Overflow
- Fragmentação de memória
- Vazamentos de memória

## Recursos de Aprendizado

### Vídeos Recomendados
1. [Memory & Storage: Crash Course Computer Science](https://www.youtube.com/watch?v=TQCr9RV7twk)
2. [How computer memory works](https://www.youtube.com/watch?v=p3q5zWCw8J4)

### Livros
1. "Understanding the Linux Virtual Memory Manager" por Mel Gorman
2. "What Every Programmer Should Know About Memory" por Ulrich Drepper

### Artigos
1. [Memory Management in Operating System](https://www.geeksforgeeks.org/memory-management-in-operating-system/)
2. [Virtual Memory in Operating System](https://www.geeksforgeeks.org/virtual-memory-in-operating-system/)

## Exercícios Práticos
1. Criar programas que demonstrem diferentes tipos de alocação de memória
2. Analisar o uso de memória em diferentes linguagens de programação
3. Identificar e corrigir memory leaks em código