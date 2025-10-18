# Go (Golang)

## Lógica de Programação

### Conceitos Básicos
- **Tipos de Dados**
  - Básicos: bool, string, int, float64
  - Compostos: array, slice, map, struct
  - Interface{}
- **Controle de Fluxo**
  - if/else
  - switch
  - for (único loop em Go)
  - defer
- **Funções**
  - Funções nomeadas
  - Funções anônimas
  - Closures
  - Métodos

### Vídeos Recomendados
1. [Go Lang Course](https://www.youtube.com/watch?v=YS4e4q9oBaU)
2. [Learn Go Programming](https://www.youtube.com/watch?v=75lJDVT1h0s)
3. [Go Tutorial Full Course](https://www.youtube.com/watch?v=rpN1Ie6ZpG0)

### Livros
1. "Go Programming Language" por Alan A. A. Donovan e Brian Kernighan
2. "Learning Go" por Jon Bodner
3. "Go in Action" por William Kennedy

### Artigos
1. [Tour of Go](https://tour.golang.org/)
2. [Effective Go](https://golang.org/doc/effective_go)
3. [Go by Example](https://gobyexample.com/)

## Algoritmos e Estruturas de Dados

### Implementações em Go
1. **Estruturas de Dados**
   ```go
   // Slice (Array Dinâmico)
   numbers := make([]int, 0)
   
   // Map (Hash Table)
   dict := make(map[string]int)
   
   // Estrutura Personalizada
   type Node struct {
       Value int
       Next  *Node
   }
   ```

2. **Algoritmos Comuns**
   - Sorting (sort package)
   - Searching
   - Graph algorithms
   - Concurrent algorithms

### Vídeos Recomendados
1. [Data Structures in Go](https://www.youtube.com/watch?v=YQs6IC-vgmo)
2. [Algorithms in Go](https://www.youtube.com/watch?v=Y0PH9NCFeqE)

### Livros
1. "100 Go Mistakes and How to Avoid Them" por Teiva Harsanyi
2. "Hands-On Data Structures and Algorithms with Go" por Yogesh Sharma

### Artigos
1. [Go Data Structures](https://research.swtch.com/godata)
2. [Go Slices: usage and internals](https://blog.golang.org/slices-intro)

## Paradigmas de Programação

### Programação Procedural
- Organização do código em procedimentos
- Funções e módulos
- Exemplo:
  ```go
  func calculateArea(width, height float64) float64 {
      return width * height
  }
  ```

### Programação Funcional
- First-class functions
- Closures
- Higher-order functions
- Exemplo:
  ```go
  filter := func(arr []int, f func(int) bool) []int {
      filtered := make([]int, 0)
      for _, v := range arr {
          if f(v) {
              filtered = append(filtered, v)
          }
      }
      return filtered
  }
  ```

### Programação Orientada a Objetos

#### Abstração
```go
type Shape interface {
    Area() float64
    Perimeter() float64
}
```

#### Encapsulamento
```go
type rectangle struct {
    width  float64
    height float64
}

func NewRectangle(w, h float64) *rectangle {
    return &rectangle{width: w, height: h}
}
```

#### Composição (em vez de Herança)
```go
type Car struct {
    Vehicle
    model string
}
```

#### Polimorfismo
```go
func printArea(s Shape) {
    fmt.Printf("Area: %f\n", s.Area())
}
```

### Vídeos Recomendados
1. [Object-Oriented Programming in Go](https://www.youtube.com/watch?v=7t2alSnE2-I)
2. [Functional Programming in Go](https://www.youtube.com/watch?v=c8Fwb4KbVJM)

### Livros
1. "Mastering GO" por Mihalis Tsoukalos
2. "Network Programming with Go" por Jan Newmarch

### Artigos
1. [Go OOP](https://golang.org/doc/faq#Is_Go_an_object-oriented_language)
2. [Functional Programming in Go](https://golang.org/doc/codewalk/functions/)

## Tópicos Avançados

### Concorrência
- Goroutines
- Channels
- Select
- Mutex
- WaitGroup

### Tratamento de Erros
- Error interface
- Multiple return values
- Panic e Recover

### Ferramentas
- go fmt
- go vet
- go test
- go mod

## Exercícios Práticos

1. **Básico**
   - Implementar uma calculadora simples
   - Criar um programa de lista de tarefas
   - Desenvolver um conversor de unidades

2. **Intermediário**
   - Criar um servidor HTTP básico
   - Implementar um cliente REST
   - Desenvolver um sistema de logging

3. **Avançado**
   - Criar um microserviço com gRPC
   - Implementar um pool de workers
   - Desenvolver um cache distribuído

4. **Projetos Práticos**
   - API REST completa
   - Sistema de chat em tempo real
   - CLI para gerenciamento de tarefas
