# Kotlin Basics

## Variables

In Kotlin, there are two types of variables:

- `var`: Mutable variable whose value can be changed.
- `val`: Immutable variable whose value cannot be changed once assigned.

Example:
```java
var age = 25
val name = "John Doe"
```

## Conditions

- `if () { }`: Conditional statement for branching logic.
- `when () { }`: Kotlin's enhanced switch statement, similar to `switch` in other languages.

**If Statement**


```java
if (age >= 18) {
    println("You are an adult.")
} else {
    println("You are a minor.")
}
```

**When Expression**

```java
when (age) {
    in 0..17 -> println("You are a minor.")
    in 18..64 -> println("You are an adult.")
    else -> println("You are a senior.")
}
```

## Functions

Kotlin functions can have different return types:

- `Unit`: Denotes functions that return no meaningful value (similar to `void` in other languages).
- `String`: Denotes functions that return a string value.
Example:

```java
fun greet(name: String): String {
    return "Hello, $name!"
}

fun printMessage() :Unit {
    println("This is a message.")
}
```

## Collections and Iteration


Kotlin provides various collection types and ways to iterate over them.

**Arrays**

```java
val array = arrayOf("a", "b", "c")
```

**Lists**

```java
val list = listOf("a", "b", "c")
val mutableList = mutableListOf("a", "b", "c")

mutableList.add("d")
```


**Maps**

```java
val map = mapOf(1 to "a", 2 to "b", 3 to "c")
val mutableMap = mutableMapOf(1 to "a", 2 to "b", 3 to "c")

mutableMap.put(4, "d")

```


