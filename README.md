# Using-Inheritance-one-class-can-acquire-the-properties-of-others.

## AIM:
To write a java program that uses inheritance to acquire properties from one class and give it to other class.

## PROCEDURE:
1. Define a class called Animal with a private name attribute and a constructor that takes the name as a parameter.
2. Within the Animal class, define a method named eat() that prints the name followed by " is eating."
3. Define a class called Dog that extends the Animal class.
4. Within the Dog class, define a constructor that takes the name as a parameter and calls the superclass constructor using the super() keyword.
5. Within the Dog class, define a method named bark() that prints "Woof! Woof!".
6. Define a class called Inherit.
7. Within the Inherit class, define the main() method.
8. Inside the main() method, create an instance of the Dog class called dog with the name "Max".
9. Call the eat() method on the dog instance.
10. Call the bark() method on the dog instance.

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
```
C:\Users\Dell\.jdks\openjdk-19.0.2\bin\java.exe "-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\lib\idea_rt.jar=10987:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\bin" -Dfile.encoding=UTF-8 -Dsun.stdout.encoding=UTF-8 -Dsun.stderr.encoding=UTF-8 -classpath "C:\Users\Dell\IdeaProjects\java full stack\out\production\java full stack" Inherit
Max is eating.
Woof! Woof!
Process finished with exit code 0
```
## RESULT:
Thus the java program to use inheritance to acquire properties from one class and give it to other class is created and the output is verifed.


