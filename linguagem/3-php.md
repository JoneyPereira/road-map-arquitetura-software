# PHP

## Lógica de Programação

### Conceitos Básicos
- **Tipos de Dados**
  - Escalares: bool, int, float, string
  - Compostos: array, object, callable
  - Especiais: NULL, resource
- **Controle de Fluxo**
  - if/else/elseif
  - switch/match
  - for, foreach, while, do-while
  - continue/break
- **Funções**
  - Funções nomeadas
  - Funções anônimas
  - Arrow functions
  - Closures

### Vídeos Recomendados
1. [PHP Tutorial for Beginners](https://www.youtube.com/watch?v=OK_JCtrrv-c)
2. [PHP Full Course](https://www.youtube.com/watch?v=6EukZDFE_Zg)
3. [Modern PHP Development](https://www.youtube.com/watch?v=2eebptXfEvw)

### Livros
1. "PHP and MySQL Web Development" por Luke Welling
2. "Modern PHP" por Josh Lockhart
3. "PHP: The Right Way" (online book)

### Artigos
1. [PHP Manual](https://www.php.net/manual/en/)
2. [PHP: The Right Way](https://phptherightway.com/)
3. [PHP Best Practices](https://phpbestpractices.org/)

## Algoritmos e Estruturas de Dados

### Implementações em PHP
1. **Estruturas de Dados**
   ```php
   // Array
   $array = [];
   
   // Objeto
   class Node {
       public $value;
       public $next;
       
       public function __construct($value) {
           $this->value = $value;
           $this->next = null;
       }
   }
   ```

2. **SPL (Standard PHP Library)**
   - SplStack
   - SplQueue
   - SplHeap
   - SplFixedArray

### Vídeos Recomendados
1. [Data Structures in PHP](https://www.youtube.com/watch?v=t2CEgPsws3U)
2. [PHP Algorithms Tutorial](https://www.youtube.com/watch?v=WX0MDWfvF0o)

### Livros
1. "PHP 7 Data Structures and Algorithms" por Mizanur Rahman
2. "Mastering PHP Design Patterns" por Junade Ali

### Artigos
1. [PHP SPL Data Structures](https://www.php.net/manual/en/spl.datastructures.php)
2. [PHP Array Functions](https://www.php.net/manual/en/ref.array.php)

## Paradigmas de Programação

### Programação Procedural
- Funções e procedimentos
- Include e require
- Escopo de variáveis
- Exemplo:
  ```php
  function calculateArea($width, $height) {
      return $width * $height;
  }
  ```

### Programação Orientada a Objetos

#### Abstração
```php
abstract class Shape {
    abstract public function area(): float;
    abstract public function perimeter(): float;
}
```

#### Herança
```php
class Rectangle extends Shape {
    private $width;
    private $height;
    
    public function __construct($width, $height) {
        $this->width = $width;
        $this->height = $height;
    }
    
    public function area(): float {
        return $this->width * $this->height;
    }
}
```

#### Polimorfismo
```php
interface Drawable {
    public function draw();
}

class Circle implements Drawable {
    public function draw() {
        // Implementation
    }
}
```

#### Encapsulamento
```php
class BankAccount {
    private $balance;
    
    public function deposit($amount) {
        if ($amount > 0) {
            $this->balance += $amount;
        }
    }
}
```

### Programação Funcional
- First-class functions
- Anonymous functions
- Array functions (map, filter, reduce)
- Exemplo:
  ```php
  $numbers = [1, 2, 3, 4, 5];
  $doubled = array_map(fn($n) => $n * 2, $numbers);
  ```

### Vídeos Recomendados
1. [PHP OOP Tutorial](https://www.youtube.com/watch?v=Anz0ArcQ5kI)
2. [Functional Programming in PHP](https://www.youtube.com/watch?v=K9qQvcsKtQk)

### Livros
1. "PHP Objects, Patterns, and Practice" por Matt Zandstra
2. "Clean PHP" por Peter MacIntyre

### Artigos
1. [PHP OOP Concepts](https://www.php.net/manual/en/language.oop5.php)
2. [PHP Design Patterns](https://refactoring.guru/design-patterns/php)

## Tópicos Avançados

### Frameworks
- Laravel
- Symfony
- CodeIgniter
- Slim

### Gerenciamento de Dependências
- Composer
- Packagist
- Autoloading

### Segurança
- SQL Injection
- XSS
- CSRF
- Password Hashing

### Performance
- Caching
- Profiling
- Otimização de consultas
- Opcache

## Exercícios Práticos

1. **Básico**
   - Criar um CRUD simples
   - Implementar um sistema de login
   - Desenvolver um blog básico

2. **Intermediário**
   - API REST com autenticação
   - Sistema de upload de arquivos
   - Integração com banco de dados

3. **Avançado**
   - CMS completo
   - E-commerce básico
   - Sistema de microserviços

4. **Projetos Práticos**
   - Sistema de gestão empresarial
   - Plataforma de cursos online
   - Rede social simples