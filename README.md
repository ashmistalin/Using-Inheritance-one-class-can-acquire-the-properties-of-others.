# Using-Inheritance-one-class-can-acquire-the-properties-of-others.

## PROGRAM:
```
class Animal {
    private String name;

    public Animal(String name) {
        this.name = name;
    }

    public void eat() {
        System.out.println(name + " is eating.");
    }
}

class Dog extends Animal {
    public Dog(String name) {
        super(name);
    }

    public void bark() {
        System.out.println("Woof! Woof!");
    }
}

public class Inherit {
    public static void main(String[] args) {
        Dog dog = new Dog("Max");
        dog.eat();
        dog.bark();
    }
}
```

## OUTPUT:
