# OOPs

## 6 Main Pillars of OOPs

### Class
- Collection of objects.
- Not a real-world entity.
- Doesn't occupy space.

### Object and Methods
- Instance of class.
- Occupy space.
- Real-world entity.

### Inheritance
- To inherit the properties of parent class.
- Advantages:
  - Code reusability.
  - Polymorphism.
- Tightly coupled.

#### Types of Inheritance
- Single
- Multilevel
- Hierarchical
- Multiple
- Hybrid

- Constructors and private functions are not inherited.

### Abstraction
- Hiding internal implementation.

### Polymorphism
- Compile Time (Static)
  - Method Overloading
  - Same name, same class, different arguments.

- Run Time (Dynamic)
  - Method Overriding
  - Inheritance, different class, same name, same arguments.

- `super` keyword
  - Parent class method.

### Encapsulation
- Information hiding.
- Wrapping variables and methods in a single unit.

### Access Modifiers
- `public` → Any package.
- `private` → Class.
- `protected` → Same package or different package with inheritance.
- `default` → Only that package.

### Abstract Class and Interface
- `implements` is used to inherit interface.

### `final` Keyword
- Value can't be changed.
- Cannot override final method.
- Can't extend or inherit final class.

### Static Variable
- Class level.
- Static methods can be called directly via class name.
- Static method can access only static data.
- Static method can't refer to `this` or `super`.
