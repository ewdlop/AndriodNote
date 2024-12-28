Sure! If you're transitioning from Java to Kotlin, it might be helpful to see how common Java constructs and idioms translate into Kotlin. Below are some examples of how you can write typical Java code in Kotlin.

### 1. Hello World

#### Java

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

#### Kotlin

```kotlin
fun main() {
    println("Hello, World!")
}
```

### 2. Variables

#### Java

```java
public class Variables {
    public static void main(String[] args) {
        int number = 10;
        String greeting = "Hello";
        System.out.println(number);
        System.out.println(greeting);
    }
}
```

#### Kotlin

```kotlin
fun main() {
    val number = 10 // 'val' is used for immutable variables
    val greeting = "Hello"
    println(number)
    println(greeting)
}
```

### 3. Functions

#### Java

```java
public class Functions {
    public static void main(String[] args) {
        int result = add(5, 3);
        System.out.println(result);
    }

    public static int add(int a, int b) {
        return a + b;
    }
}
```

#### Kotlin

```kotlin
fun main() {
    val result = add(5, 3)
    println(result)
}

fun add(a: Int, b: Int): Int {
    return a + b
}
```

### 4. Classes and Objects

#### Java

```java
public class Person {
    private String name;

    public Person(String name) {
        this.name = name;
    }

    public String getName() {
        return name;
    }

    public static void main(String[] args) {
        Person person = new Person("John");
        System.out.println(person.getName());
    }
}
```

#### Kotlin

```kotlin
class Person(val name: String)

fun main() {
    val person = Person("John")
    println(person.name)
}
```

### 5. Conditionals

#### Java

```java
public class Conditionals {
    public static void main(String[] args) {
        int number = 10;
        if (number > 0) {
            System.out.println("Positive");
        } else if (number < 0) {
            System.out.println("Negative");
        } else {
            System.out.println("Zero");
        }
    }
}
```

#### Kotlin

```kotlin
fun main() {
    val number = 10
    if (number > 0) {
        println("Positive")
    } else if (number < 0) {
        println("Negative")
    } else {
        println("Zero")
    }
}
```

### 6. Loops

#### Java

```java
public class Loops {
    public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
            System.out.println(i);
        }
    }
}
```

#### Kotlin

```kotlin
fun main() {
    for (i in 0 until 5) {
        println(i)
    }
}
```

### 7. Lists

#### Java

```java
import java.util.ArrayList;
import java.util.List;

public class Lists {
    public static void main(String[] args) {
        List<String> list = new ArrayList<>();
        list.add("A");
        list.add("B");
        list.add("C");
        for (String item : list) {
            System.out.println(item);
        }
    }
}
```

#### Kotlin

```kotlin
fun main() {
    val list = listOf("A", "B", "C")
    for (item in list) {
        println(item)
    }
}
```

### Summary

- **Kotlin is more concise**: Kotlin eliminates boilerplate code, making it more concise and readable.
- **Type Inference**: Kotlin has strong type inference which means you don't always need to specify the type explicitly.
- **Immutable by Default**: Variables declared with `val` are immutable, encouraging functional programming practices.

These examples should give you a good starting point to understand how Java code translates into Kotlin. If you have any specific Java code that you want to see in Kotlin, feel free to ask!
