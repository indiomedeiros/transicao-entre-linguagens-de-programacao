# Tabela de Transição: Java → JavaScript

## Comparação Geral

| Conceito               | Java                          | JavaScript                                 |
| ---------------------- | ----------------------------- | ------------------------------------------ |
| Arquivo                | `Main.java`                   | `app.js`                                   |
| Execução               | Compilado para bytecode JVM   | Interpretado/JIT pelo navegador ou Node.js |
| Tipagem                | Estática                      | Dinâmica                                   |
| Declaração de variável | `int idade = 25;`             | `let idade = 25;`                          |
| Constante              | `final double PI = 3.14;`     | `const PI = 3.14;`                         |
| String                 | `String nome = "Maria";`      | `let nome = "Maria";`                      |
| Número decimal         | `double salario = 1500.50;`   | `let salario = 1500.50;`                   |
| Booleano               | `boolean ativo = true;`       | `let ativo = true;`                        |
| Comentário linha       | `// comentário`               | `// comentário`                            |
| Comentário bloco       | `/* comentário */`            | `/* comentário */`                         |
| Condicional            | `if`                          | `if`                                       |
| Senão                  | `else`                        | `else`                                     |
| Múltiplas opções       | `switch`                      | `switch`                                   |
| Laço de repetição      | `for`                         | `for`                                      |
| Enquanto               | `while`                       | `while`                                    |
| Faça enquanto          | `do...while`                  | `do...while`                               |
| Função/Método          | `public static void metodo()` | `function metodo()`                        |
| Retorno                | `return`                      | `return`                                   |
| Vetor                  | `int[] numeros`               | `let numeros = []`                         |
| Lista                  | `ArrayList`                   | `Array`                                    |
| Classe                 | `class Pessoa`                | `class Pessoa`                             |
| Herança                | `extends`                     | `extends`                                  |
| Interface              | `interface`                   | Não possui (use TypeScript para interfaces)|
| Tratamento de erro     | `try/catch`                   | `try/catch`                                |
| Impressão no console   | `System.out.println()`        | `console.log()`                            |
| Entrada de dados       | `Scanner`                     | `prompt()` (navegador) / `readline` (Node) |
| Valor nulo             | `null`                        | `null`                                     |
| Ausência de valor      | Não existe                    | `undefined`                                |

---

# Olá Mundo

## Java

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Olá Mundo!");
    }
}
```

## JavaScript

```javascript
console.log("Olá Mundo!");
```

---

# Variáveis

## Java

```java
String nome = "Ana";
int idade = 20;
double salario = 2500.50;
boolean ativo = true;
```

## JavaScript

```javascript
let nome = "Ana";
let idade = 20;
let salario = 2500.50;
let ativo = true;
```

---

# Constantes

## Java

```java
final double PI = 3.14159;
```

## JavaScript

```javascript
const PI = 3.14159;
```

---

# Condicionais

## Java

```java
if (idade >= 18) {
    System.out.println("Maior de idade");
} else {
    System.out.println("Menor de idade");
}
```

## JavaScript

```javascript
if (idade >= 18) {
    console.log("Maior de idade");
} else {
    console.log("Menor de idade");
}
```

---

# Switch

## Java

```java
switch (dia) {
    case 1:
        System.out.println("Domingo");
        break;
    case 2:
        System.out.println("Segunda");
        break;
    default:
        System.out.println("Outro dia");
}
```

## JavaScript

```javascript
switch (dia) {
    case 1:
        console.log("Domingo");
        break;
    case 2:
        console.log("Segunda");
        break;
    default:
        console.log("Outro dia");
}
```

---

# Laço For

## Java

```java
for (int i = 0; i < 5; i++) {
    System.out.println(i);
}
```

## JavaScript

```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

---

# Laço While

## Java

```java
int contador = 0;

while (contador < 5) {
    System.out.println(contador);
    contador++;
}
```

## JavaScript

```javascript
let contador = 0;

while (contador < 5) {
    console.log(contador);
    contador++;
}
```

---

# Laço Do While

## Java

```java
int contador = 0;

do {
    System.out.println(contador);
    contador++;
} while (contador < 5);
```

## JavaScript

```javascript
let contador = 0;

do {
    console.log(contador);
    contador++;
} while (contador < 5);
```

---

# Funções

## Java

```java
public static int somar(int a, int b) {
    return a + b;
}
```

## JavaScript

```javascript
function somar(a, b) {
    return a + b;
}
```

---

# Arrays

## Java

```java
int[] numeros = {1, 2, 3, 4, 5};

System.out.println(numeros[0]);
```

## JavaScript

```javascript
let numeros = [1, 2, 3, 4, 5];

console.log(numeros[0]);
```

---

# Listas

## Java

```java
import java.util.ArrayList;

ArrayList<String> nomes = new ArrayList<>();

nomes.add("Ana");
nomes.add("João");
```

## JavaScript

```javascript
let nomes = [];

nomes.push("Ana");
nomes.push("João");
```

---

# Objetos

## Java

```java
// Objeto criado a partir de uma classe
Pessoa pessoa = new Pessoa();
pessoa.nome = "Ana";
pessoa.idade = 20;
```

## JavaScript

```javascript
// Objeto literal: criado diretamente, sem precisar de uma classe
let pessoa = {
    nome: "Ana",
    idade: 20
};
```

> **Nota:** Em JavaScript, objetos podem ser criados diretamente como literais, sem a necessidade de uma classe. Isso não tem equivalente direto em Java.

---

# Classes

## Java

```java
public class Pessoa {

    String nome;

    public Pessoa(String nome) {
        this.nome = nome;
    }

    public void apresentar() {
        System.out.println(nome);
    }
}
```

## JavaScript

```javascript
class Pessoa {

    constructor(nome) {
        this.nome = nome;
    }

    apresentar() {
        console.log(this.nome);
    }
}
```

---

# Herança

## Java

```java
class Animal {
    void emitirSom() {
        System.out.println("Som");
    }
}

class Cachorro extends Animal {
}
```

## JavaScript

```javascript
class Animal {
    emitirSom() {
        console.log("Som");
    }
}

class Cachorro extends Animal {
}
```

---

# Tratamento de Exceções

> **Atenção:** Em Java, `10 / 0` com inteiros lança `ArithmeticException`. Em JavaScript, **isso não acontece** — o resultado é `Infinity`, sem erro. Os exemplos abaixo usam situações que realmente lançam erros em cada linguagem.

## Java

```java
try {
    int resultado = 10 / 0; // lança ArithmeticException
} catch (Exception e) {
    System.out.println("Erro: " + e.getMessage());
}
```

## JavaScript

```javascript
try {
    null.propriedade; // lança TypeError: Cannot read properties of null
} catch (erro) {
    console.log("Erro: " + erro.message);
}
```

> Em JavaScript, `10 / 0` retorna `Infinity` e **não** lança exceção. Use `try/catch` para erros reais, como acessar propriedades de `null` ou `undefined`, ou usar `JSON.parse()` com dados inválidos.

---

# Entrada de Dados

## Java

```java
import java.util.Scanner;

Scanner scanner = new Scanner(System.in);

String nome = scanner.nextLine();
```

## JavaScript (Navegador)

```javascript
let nome = prompt("Digite seu nome:");
```

## JavaScript (Node.js)

```javascript
const readline = require("readline");

const rl = readline.createInterface({ input: process.stdin });

rl.question("Digite seu nome: ", (nome) => {
    console.log("Olá, " + nome);
    rl.close();
});
```

> `prompt()` só funciona no navegador. No Node.js, use o módulo `readline` ou bibliotecas como `inquirer`.

---

# Tipagem

## Java (Tipagem Estática)

```java
String valor = "10";

// Erro de compilação
// valor = 10;
```

## JavaScript (Tipagem Dinâmica)

```javascript
let valor = "10";

valor = 10;
valor = true;
valor = [];
```

---

# Principais Diferenças

| Java                              | JavaScript                        |
| --------------------------------- | --------------------------------- |
| Tipagem estática                  | Tipagem dinâmica                  |
| Compilado para JVM                | Executado no navegador ou Node.js |
| Classes obrigatórias              | Classes opcionais                 |
| Mais verboso                      | Mais conciso                      |
| Forte uso de orientação a objetos | Multiparadigma                    |
| ArrayList para listas             | Array nativo                      |
| Scanner para entrada              | `prompt()` (navegador) ou `readline` / `inquirer` (Node.js) |
| `10 / 0` lança `ArithmeticException` | `10 / 0` retorna `Infinity`    |

---

# Resumo para Quem Vem do Java

1. Troque `System.out.println()` por `console.log()`.
2. Troque `ArrayList` por `Array`.
3. Troque tipos (`int`, `String`, `double`) por `let` ou `const`.
4. Entenda que o tipo de uma variável pode mudar durante a execução.
5. Objetos literais são amplamente utilizados — não precisam de uma classe.
6. Nem tudo precisa estar dentro de uma classe.
7. JavaScript é multiparadigma: procedural, orientado a objetos e funcional.
8. Divisão por zero **não lança erro** em JavaScript — retorna `Infinity`.

> JavaScript não é uma versão simplificada de Java. São linguagens diferentes que compartilham parte da sintaxe básica, mas possuem filosofias, ecossistemas e formas de execução distintas.
