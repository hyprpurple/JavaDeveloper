### 📘 Enumerations. Creation, Use, and Advantages. Wrapper Classes

---

### 📃 Description
- Enumerations in Java
- Creation and Application of Enumerations
- Wrapper Classes
- Instantiation of Wrapper Classes
- Autoboxing and Unboxing

---

### 📜 Enumerations in Java

**Enumerations (enum)** are data types that allow programmers to define a predefined set of constant values. They offer an elegant and safe solution for limiting the values that a variable can take, eliminating the need for manual checks and reducing the risk of errors.

Enumerations are useful for representing logical groups of values, such as days of the week, months of the year, or fuel types.

---

### 🔍 Creation and Application of Enumerations

#### Creating an Enumeration. For example, we'll define an enumeration for fuel types:

- The `FuelType` enumeration is declared with three values: `DIESEL`, `GASOLINE`, and `PROPANE`.

- Enumerations are created using the `enum` keyword.

```java
public enum FuelType {
    DIESEL, GASOLINE, PROPANE
}
```

#### Using the Enumeration in a Class:

- The `FuelStation` class defines an attribute `fuelType` of type `FuelType`.

- The `FuelStation` class constructor takes a `FuelType` parameter to initialize the attribute.

- The `displayFuelType` method displays the current value of `fuelType`.

```java
public class FuelStation {
    private FuelType fuelType;

    public FuelStation(FuelType fuelType) {
      this.fuelType = fuelType;
    }
  
    public void displayFuelType() {
      System.out.println("Fuel type: " + fuelType);
    }
}
```

- In the `main` method, three `FuelStation` objects are created with different fuel types, and the `displayFuelType` method is called for each object.

```java
public class Main {
    public static void main(String[] args) {
        FuelStation fuelStation = new FuelStation(FuelType.GASOLINE);
        fuelStation.displayFuelType();
    }
}
```

---

### 💻 Wrapper Classes

In Java, there are two types of data: primitive and reference (objects). In most cases, numeric values, characters, and boolean values are used as primitives because they are more memory-efficient.

However, there are situations where it is important for a primitive value to be treated as an object. For this purpose, Java provides a set of classes called Wrapper classes, which are containers for primitive values. Thus, for each primitive data type in Java, there is a corresponding Wrapper class:

| Primitive <br/> Data Type | Reference <br/> Data Type | Example Usage          |
|---------------------------|----------------------------|------------------------|
| byte                      | Byte                       | `new Byte((byte) 1)`   |
| short                     | Short                      | `new Short((short) 1)` |
| int                       | Integer                    | `new Integer(1)`       |
| long                      | Long                       | `new Long(1)`          |
| float                     | Float                      | `new Float(1.0)`       |
| double                    | Double                     | `new Double(1.0)`      |
| boolean                   | Boolean                    | `new Boolean(true)`    |
| char                      | Character                  | `new Character('c')`   |

<br/>

---

### 📦 Creation and Application of Wrapper Classes

Wrapper classes can be created in three ways:

- Using the class constructor

```java
Integer intWrapper = new Integer(34);
```

- Using the `valueOf()` method 

```java
Float floatWrapper = Float.valueOf("3.14f");
```

- By assigning a primitive value to a reference variable 

```java
Short shortWrapper = 404;
```

---

### 🔍 Autoboxing and Unboxing

- **Autoboxing** is the process where Java automatically converts a primitive value into an object of the Wrapper class without explicitly calling constructors.

- **Unboxing** is the reverse process: automatically extracting the primitive value from a Wrapper object without explicitly calling methods.

```java
Integer integerWrapper = 404;          // Autoboxing

int integerPrimitive = integerWrapper; // Unboxing
```

---

<br>
    <h1 align="center">
     🏆 Quiz 🏆
    </h1>
<br/>

**Question 1: What term is used to describe the process of converting a `Wrapper` object back to a primitive?**
- Boxing
- Unboxing
- Autoboxing

<details>
    <br/><p><strong>Answer: </strong>Unboxing</p><br/>
</details>

**Question 2: Which of the following methods are valid methods of the `Integer` class that can be used to extract a primitive value from an object?**
- `intvalue()`
- `IntValue()`
- `intValue()`
- `valueOf()`

<details>
    <br/><p><strong>Answer: </strong><code>intValue()</code></p><br/>
</details>

**Question 3: The purpose of an enumeration is to store:**
- Values entered by the user from the console
- Values that frequently change in the program
- Constant values

<details>
    <br/><p><strong>Answer: </strong>Constant values</p><br/>
</details>

**Question 4: The keyword used to define an enumeration is:**
- `enum`
- `enumeration`
- `Enum`

<details>
    <br/><p><strong>Answer: </strong><code>enum</code></p><br/>
</details>
