# Kotlin

## Lógica de Programação

### Conceitos Básicos
- **Tipos de Dados**
  - Básicos: Int, Long, Float, Double, Boolean, String
  - Nullable Types: Int?, String?
  - Arrays e Collections
  - Data Classes
- **Controle de Fluxo**
  - if/else como expressão
  - when (switch aprimorado)
  - for, while, do-while
  - Ranges (1..10)
- **Funções**
  - Top-level functions
  - Extension functions
  - Infix functions
  - Higher-order functions

### Vídeos Recomendados
1. [Kotlin Course for Beginners](https://www.youtube.com/watch?v=F9UC9DY-vIU)
2. [Kotlin Tutorial for Beginners](https://www.youtube.com/watch?v=wuiT4T_LJQo)
3. [Kotlin Programming Fundamentals](https://www.youtube.com/watch?v=AeC4G-H-MQA)

### Livros
1. "Kotlin in Action" por Dmitry Jemerov e Svetlana Isakova
2. "Head First Kotlin" por Dawn Griffiths e David Griffiths
3. "Programming Kotlin" por Venkat Subramaniam

### Artigos
1. [Kotlin Official Documentation](https://kotlinlang.org/docs/home.html)
2. [Kotlin by Example](https://play.kotlinlang.org/byExample/overview)
3. [Kotlin Koans](https://kotlinlang.org/docs/koans.html)

## Algoritmos e Estruturas de Dados

### Implementações em Kotlin
1. **Estruturas de Dados**
   ```kotlin
   // Lista Mutável
   val list = mutableListOf<Int>()
   
   // Map Mutável
   val map = mutableMapOf<String, Int>()
   
   // Classe Nó para Lista Encadeada
   data class Node<T>(
       var value: T,
       var next: Node<T>? = null
   )
   ```

2. **Algoritmos Comuns**
   - Collections.sort()
   - binarySearch
   - Collections utilities
   - Sequence operations

### Vídeos Recomendados
1. [Data Structures in Kotlin](https://www.youtube.com/watch?v=ay_m5WRHrPM)
2. [Algorithms with Kotlin](https://www.youtube.com/watch?v=JN5a7xA5x3k)

### Livros
1. "Kotlin Standard Library Cookbook" por Samuel Urbanowicz
2. "Hands-On Data Structures and Algorithms with Kotlin" por Chandra Sekhar Nayak

### Artigos
1. [Kotlin Collections Overview](https://kotlinlang.org/docs/collections-overview.html)
2. [Sequences](https://kotlinlang.org/docs/sequences.html)

## Paradigmas de Programação

### Programação Funcional
- Funções de primeira classe
- Lambdas
- High-order functions
- Exemplo:
  ```kotlin
  val sum = { x: Int, y: Int -> x + y }
  fun <T, R> List<T>.map(transform: (T) -> R): List<R>
  ```

### Programação Orientada a Objetos

#### Abstração
```kotlin
interface Shape {
    fun area(): Double
    fun perimeter(): Double
}
```

#### Herança
```kotlin
open class Animal(val name: String) {
    open fun makeSound() = println("Some sound")
}

class Dog(name: String): Animal(name) {
    override fun makeSound() = println("Woof!")
}
```

#### Polimorfismo
```kotlin
fun printArea(shape: Shape) {
    println("Area: ${shape.area()}")
}
```

#### Encapsulamento
```kotlin
class BankAccount {
    private var balance = 0.0
    
    fun deposit(amount: Double) {
        if (amount > 0) balance += amount
    }
}
```

### Programação Multiparadigma
- Mistura de OOP e Funcional
- Data Classes
- Sealed Classes
- Extension Functions

### Vídeos Recomendados
1. [Functional Programming with Kotlin](https://www.youtube.com/watch?v=r-E6wH7qZlY)
2. [Object-Oriented Programming in Kotlin](https://www.youtube.com/watch?v=9QW7-xJ5X6E)

### Livros
1. "Functional Programming in Kotlin" por Marco Vermeulen
2. "Object-Oriented Programming in Kotlin" por Gavin King

### Artigos
1. [Kotlin OOP Guide](https://kotlinlang.org/docs/classes.html)
2. [Functional Programming with Kotlin](https://kotlinlang.org/docs/lambdas.html)

## Tópicos Avançados

### Coroutines
- Básico de coroutines
- Dispatchers
- Flow
- Channels
- Job e Deferred

### Interoperabilidade com Java
- Chamando código Java
- Anotações específicas
- Null-safety
- Properties

### Android Development
- Jetpack Compose
- Android KTX
- ViewModel
- Room

## Exercícios Práticos

1. **Básico**
   - Implementar uma calculadora com interface de texto
   - Criar um gerenciador de contatos
   - Desenvolver um conversor de moedas

2. **Intermediário**
   - Criar uma API REST com Ktor
   - Implementar um cliente HTTP
   - Desenvolver um CRUD com banco de dados

3. **Avançado**
   - Criar um app Android com Jetpack Compose
   - Implementar um chat usando coroutines
   - Desenvolver uma biblioteca multiplatforma

4. **Projetos Práticos**
   - Backend completo com Spring Boot
   - Aplicativo Android com arquitetura MVVM
   - CLI multiplataforma