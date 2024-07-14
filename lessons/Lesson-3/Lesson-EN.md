### 📘 Basic Concepts in Java: Syntax, Variables, Data Types, Operators

---

### 📃 Description
- Java Classes
- Executable and Non-executable Classes
- Main Method
- Java Packages
- Import Declaration
- Comments
- Primitive Data Types
- Operators

---

### 📚 Java Classes

**Class** — is a **fundamental concept of object-oriented programming**. In the Java programming language, a class
represents the definition of objects, which includes attributes (data) and methods (possible operations on the data).
In other words, a class is a blueprint for creating objects of the same type.

---

### 🚀 Executable and Non-executable Classes

In Java, a program must have one or more classes.

- To be executable, a program must have a `main` **method, which serves as the entry point for the program**.
Such a class is called executable.

- If a class does **not contain a** `main` **method, it cannot be run directly** and is called non-executable.

#### Example of an executable class:

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello world!");
    }
}
```

<br/>

#### Example of a non-executable class:

```java
public class Hello {
    public static void sayHelloWorld() {
        System.out.println("Hello world!");
    }
}
```

<br/>

---

### 💻 Main method

Execution of any Java program starts with the `main` method, defined as follows:

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello world!");
    }
}
```

Here are three equivalent definitions of the `main` method:

```java
public static void main(String[] args) { }
```

```java
public static void main(String args[]) { }
```

```java
public static void main(String... args) { }
```


---

### 📦 Java Packages

Every Java class belongs to a package. Packages in Java are used for logically grouping source code and determining the
accessibility of various classes in a program.

```java
package javadeveloper.lessons;

public class Main {
    public static void main(String[] args) {
        System.out.println("Hello world!");
    }
}
```

---

### 🔍 Import Declaration

An import statement specifies the package from which a class is imported, along with the imported class name:

```java
import javadeveloper.lessons;
```

---

### 📝 Comments

In programming, comments are used to document sequences of code.

```java
public class Main {
    public static void main(String[] args) {
        // Display "Hello world!" to console
        System.out.println("Hello world!");
    }
}
```

In programming, comments are used to document sequences of code:

- Single-line comments start with `//`.


- Multi-line comments start with `/*` and end with `*/`.


- JavaDoc comments are special comments used for documenting a class or method. They start with `/**` and end with `*/`.

---

### 📊 Primitive Data Types

Primitive data types, as the name implies, are the simplest data types in the programming language. In Java,
the following eight primitive data types are defined:

- `byte` — Stores integer numbers from -128 to 127. Typically used for saving memory when working with large arrays of numbers.


- `short` — Stores integer numbers from -32,768 to 32,767. Provides a larger range of values compared to `byte`.


- `int` — Primary type for storing integer numbers in Java. Stores numbers from -2,147,483,648 to 2,147,483,647.


- `long` — Used for storing very large integer numbers. Range from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807.


- `float` — Stores single-precision floating-point numbers. Used for numbers with a decimal part.


- `double` — Used for storing double-precision floating-point numbers. Provides greater precision compared to float.


- `char` — Used for storing a single Unicode character (e.g., letters, digits, punctuation marks).


- `boolean` — Used for storing `true` or `false` values.

<br/>

#### Integer

| Type  | Memory Allocation | Value Range                                             |
|-------|-------------------|---------------------------------------------------------|
| byte  | 8 bits            | -128 to 128                                             |
| short | 16 bits           | -32.768 to 32.768                                       |
| int   | 32 bits           | -2.147.483.648 to 2.147.483.648                         |
| long  | 64 bits           | -9.223.372.036.854.775.808 to 9.223.372.036.854.775.808 |

<br/>

#### Floating Point

| Type   | Memory Allocation | Value Range                                                |
|--------|-------------------|------------------------------------------------------------|
| float  | 32 bits           | +/–1.4E–45 la +/–3.4028235E+38, +/–∞, +/–0, NaN            |
| double | 64 bits           | +/–4.9E–324 la +/–1.7976931348623157E+308, +/–∞, +/–0, NaN |

<br/>

#### Character

| Type | Memory Allocation |
|------|-------------------|
| char | 16 bits           |

<br/>

#### Логический

| Type    | Memory Allocation |
|---------|-------------------|
| boolean | 8 bits            |

<br/>

---

### ➕ Operators

Java has four categories of operators that can be used to manipulate variable values:

- **Arithmetic operators** — Used for mathematical operations.

- **Assignment operators** — Used for assigning values to variables.

- **Comparison operators** — Used for comparing two values.

- **Logical operators** — Used for evaluating logical conditions.

<br/>

| Type       | Operators                           |
|------------|-------------------------------------|
| Arithmetic | `+`, `-`, `*`, `/`, `%`, `++`, `--` |
| Assignment | `=`, `+=`, `-=`, `*=`, `/=`         |
| Comparison | `<`, `<=`, `>`, `>=`, `==`, `!=`    |
| Logical    | `!`, `&&`, ``\|\|``                 |

<br/>

---

<br>
    <h1 align="center">
     🏆 Quiz 🏆
    </h1>
<br/>

**Question 1: Difference between executable and non-executable class:**
- Executable class is written in another project.
- Executable class has a method that serves as the entry point for the program.
- There is no difference.

<details>
    <br/><p><strong>Answer: </strong>Executable class has a method that serves as the entry point for the program</p><br/>
</details>

**Question 2: Java bytecode is interpreted by:**
- JRE
- JDK
- JVM

<details>
    <br/><p><strong>Answer: </strong>JVM</p><br/>
</details>

**Question 3: The entry point for any Java program is in the method:**
- `Main`
- `main`
- `start`

<details>
    <br/><p><strong>Answer: </strong><code>main</code></p><br/>
</details>

**Question 4: Correct declaration of the `main` method is:**
- `public final void main(String[] args) { ... }`

- `public static void main(String args) { ... }`

- `public static void main(String[] args) { ... }`

<details>
    <br/><p><strong>Answer: </strong><code>public static void main(String[] args) { ... }</code></p><br/>
</details>
