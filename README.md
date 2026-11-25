# Object-Oriented Programming (OOP)

## 1. Class & Object

### Class
- A class is a blueprint or template used to create objects.
- It is not a real-world entity itself.
- A class defines the properties (variables) and behaviors (methods) of objects.
- A class declaration itself doesn't allocate memory for instance variables; memory is allocated when objects are created.

### Object
- An object is an instance of a class.
- It represents an entity with state and behavior.
- Objects occupy memory when instantiated.
- **State** → Variables / attributes
- **Behavior** → Methods

---

## 2. Inheritance

- Inheritance allows one class to acquire the properties and behaviors of another class.
- It promotes **code reusability**.
- It supports runtime polymorphism through method overriding.
- Inheritance can create tight coupling between parent and child classes if used excessively.

### Types of Inheritance
1. Single Inheritance
2. Multilevel Inheritance
3. Hierarchical Inheritance
4. Multiple Inheritance
5. Hybrid Inheritance

> Java supports single, multilevel, and hierarchical inheritance through classes. It does not support multiple inheritance of classes, but it supports multiple inheritance through interfaces.

### Important Points
- `private` members are not directly accessible in subclasses. Private methods are not inherited in the usable sense.
- Constructors are not inherited by subclasses.
- The `super` keyword is used to access parent-class members and invoke parent constructors.

---

## 3. Abstraction

- Abstraction means **hiding internal implementation details and exposing only essential functionality**.
- It focuses on *what an object does* rather than *how it does it*.
- It can be achieved in Java using:
  - Abstract classes
  - Interfaces

---

## 4. Polymorphism

Polymorphism means **one interface or method name can represent different behaviors**.

### Compile-Time Polymorphism (Static Polymorphism)
Achieved through **method overloading**.

- Same method name
- Same class (commonly)
- Different parameter list (number, type, or order of arguments)

### Runtime Polymorphism (Dynamic Polymorphism)
Achieved through **method overriding**.

- Inheritance is involved (class inheritance or interface implementation).
- Same method signature.
- Subclass provides its own implementation.
- Method invocation is resolved at runtime based on the actual object type.

### `super` Keyword
- Used to call the parent class constructor.
- Used to access parent class methods.
- Used to access parent class variables when they are hidden by subclass variables.

---

## 5. Encapsulation

- Encapsulation means **wrapping data and methods together into a single unit (class)**.
- It also involves restricting direct access to internal data (information hiding).
- Achieved using access modifiers such as `private` and controlled access through public methods (getters, setters, or other methods).
- Getters and setters are optional; only expose methods that are required.

---

## 6. Access Modifiers

| Modifier | Accessibility |
|---|---|
| `public` | Accessible from anywhere, subject to module rules |
| `private` | Accessible only within the declaring class |
| `protected` | Accessible within the same package and in subclasses outside the package (subject to Java inheritance access rules) |
| `default` (no modifier) | Accessible only within the same package |

---

## 7. Abstract Class & Interface

### Abstract Class
- Declared using the `abstract` keyword.
- Can contain abstract and non-abstract methods.
- Can have constructors and instance variables.
- Cannot be instantiated directly.

### Interface
- Defines a contract that implementing classes must follow.
- A class uses the `implements` keyword to implement an interface.
- Supports multiple interface implementation in Java.
- Can contain abstract methods, default methods, static methods, and private helper methods (modern Java).

---

## 8. `final` Keyword

- **Final variable** → Cannot be reassigned after initialization.
- **Final method** → Cannot be overridden in subclasses.
- **Final class** → Cannot be extended / inherited.

---

## 9. `static` Keyword

- Static variables belong to the class rather than individual objects.
- Static methods can be called using the class name.
- Static methods can directly access only static members of the class.
- Static methods cannot use `this` or `super` because they don't belong to an instance.
- Static methods can access instance members through an object reference.

