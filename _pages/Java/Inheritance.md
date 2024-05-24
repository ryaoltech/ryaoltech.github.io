---
title: "Inheritance in Java"
tags:
    - Algorithms
    - OOP
    - Developer
date: "2023-09-05"
thumbnail: "/assets/img/thumbnail/java.png"
bookmark: true
---

# Inheritance in Java

Inheritance is a mechanism in object-oriented programming that allows one class to inherit the properties (fields) and behaviors (methods) of another class. This helps in reusing code and establishing a natural hierarchical relationship between classes.

## Step-by-Step Guide

### Step 1: Create the Superclass

Define a superclass (or parent class) with some fields and methods.

```java
// Superclass
public class Animal {
    // Fields
    private String name;
    private int age;

    // Constructor
    public Animal(String name, int age) {
        this.name = name;
        this.age = age;
    }

    // Method
    public void eat() {
        System.out.println(name + " is eating.");
    }

    // Getter and Setter methods
    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }
}
```

### Step 2: Create the Subclass

Define a subclass (or child class) that extends the superclass. The subclass inherits the fields and methods from the superclass.
```java
// Subclass
public class Dog extends Animal {
    // Additional field specific to Dog
    private String breed;

    // Constructor
    public Dog(String name, int age, String breed) {
        super(name, age); // Call the constructor of the superclass
        this.breed = breed;
    }

    // Additional method specific to Dog
    public void bark() {
        System.out.println(getName() + " is barking.");
    }

    // Getter and Setter methods
    public String getBreed() {
        return breed;
    }

    public void setBreed(String breed) {
        this.breed = breed;
    }
}
```

### Step 3: Use the subclass

Create an instance of the subclass and demonstrate inheritance by calling methods from both the superclass and the subclass.
```Java
public class Main {
    public static void main(String[] args) {
        // Create an instance of the Dog class
        Dog dog = new Dog("Buddy", 3, "Golden Retriever");

        // Call methods inherited from the Animal class
        dog.eat();

        // Call method specific to the Dog class
        dog.bark();

        // Access inherited fields using getter methods
        System.out.println(dog.getName() + " is a " + dog.getBreed() + ".");
        System.out.println(dog.getName() + " is " + dog.getAge() + " years old.");
    }
}

```