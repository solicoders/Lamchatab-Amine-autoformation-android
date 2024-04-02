---
layout: default
chapitre: introduction
order: 3
---


# Introduction to kotlin
![Introduction to kotlin](1-1-introduction-to-kotlin/images/kotline.svg){:width="500px" }*Introduction to kotlin*

## Basic-syntax

### Program entry point

```java
fun main() {
    println("Hello, World!")
}
```
- An entry point to a Kotlin application is the main function. You can declare it without any parameters. The return type is not specified, which means that the function returns nothing.
- println writes a line to the standard output. It is imported implicitly. Also, note that semicolons at the end of code lines are optional.


### Functions

```java
fun sum(a: Int, b: Int): Int {
    return a + b
}
```
- A function body can be an expression. Its return type is inferred.

### Variables

Read-only local variables are defined using the keyword val. They can be assigned a value only once.

```java
val a: Int = 1  // immediate assignment
val b = 2   // `Int` type is inferred
val c: Int  // Type required when no initializer is provided
c = 3       // deferred assignment
```

## Type inference

Type inference, sometimes called type reconstruction, refers to the automatic detection of the type of an expression in a formal language. These include programming languages and mathematical type systems, but also natural languages in some branches of computer science and linguistics. 


```java
fun main() {
    var nom = "Amine"
    var bonjour_nom = Bonjour(nom)
    println (bonjour_nom)
    println (nom)
}

fun Bonjour(nom:String):String{
    nom =  "Bonjour" + nom
    return nom
}
```
output : 
```java
    Val cannot be reassigned
```

10 instructions et utilise 3 variables en mémoire. Voici le décompte :

1. Déclaration de la variable nom : var nom = "Fouad"
2. Déclaration de la variable bonjour_nom : var bonjour_nom = Bonjour(nom)
3. Appel de la fonction Bonjour(nom) dans la déclaration de bonjour_nom
4. Affichage de bonjour_nom : println(bonjour_nom)
5. Affichage de nom : println(nom)
6. Déclaration de la fonction Bonjour(nom:String):String{
7. Affectation de la valeur "Bonjour" + nom à nom dans la fonction Bonjour
8. Retour de nom dans la fonction Bonjour
9. Fermeture de la fonction Bonjour
10. Fin du programme main()

Cela fait donc un total de 10 instructions. En ce qui concerne les variables utilisées en mémoire, il y en a trois :

- nom : de type String, initialisée à "Amine"
- bonjour_nom : de type String, initialisée par l'appel à la fonction Bonjour(nom)
- Variable temporaire dans la fonction Bonjour pour stocker la valeur "Bonjour" + nom

Ces trois variables sont présentes dans la mémoire pendant l'exécution du programme.

### References

[https://developer.android.com/training/kotlinplayground](https://developer.android.com/training/kotlinplayground)
