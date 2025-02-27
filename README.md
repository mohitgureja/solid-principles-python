
# SOLID Principles
Explanation and Examples for Solid Design Principles

The SOLID principles are a set of design principles intended to make software designs more understandable, flexible, and maintainable. These principles form the foundation of good object-oriented design.

---

## 1. Single Responsibility Principle (SRP)
**Definition:** A class should have only one reason to change. In other words, a class should have a single, well-defined responsibility.

- **Why?**
  Keeping each class focused on a single responsibility prevents code from becoming too complex and tightly coupled to
  multiple concerns.

- **Example:** A class that handles both business logic and UI rendering violates SRP. Instead, split these
  responsibilities into separate classes: one for business logic and another for UI.

- [Learn more about SRP in this example notebook: `srp.ipynb`](./srp.ipynb)
---

## 2. Open/Closed Principle (OCP)
**Definition:** Software entities (such as classes, modules, and functions) should be open for extension but closed for modification.

- **Why?**
  This ensures that you can extend the functionality of a module without altering its existing behavior, minimizing the risk of introducing new bugs.

- **Example:** Instead of modifying a class to add new features, use interfaces, inheritance, or composition to extend the behavior.

- [Learn more about OCP in this example notebook: `ocp.ipynb`](./ocp.ipynb)

---

## 3. Liskov Substitution Principle (LSP)
**Definition:** Subtypes should be substitutable for their base types. That is, if `S` is a subtype of `T`, objects of type `T` may be replaced with objects of type `S` without altering the correctness of the program.

- **Why?**
  This ensures that derived classes can seamlessly replace base classes without causing application errors.

- **Example:** Avoid overriding methods in derived classes in such a way that they violate the expected behavior defined in the base class.

---

## 4. Interface Segregation Principle (ISP)
**Definition:** A class should not be forced to implement interfaces it does not use. Instead, split large interfaces into smaller, more focused ones.

- **Why?**
  This prevents clients from being forced to depend on methods they do not need, enhancing flexibility and maintainability.

- **Example:** A "fat" interface with many unrelated methods should be broken into smaller, more specific interfaces.

---

## 5. Dependency Inversion Principle (DIP)
**Definition:** High-level modules should not depend on low-level modules. Instead, both should depend on abstractions. Furthermore, abstractions should not depend on details; details should depend on abstractions.

- **Why?**
  This reduces the coupling between high-level and low-level modules, making the system more reusable and easier to maintain.

- **Example:** Instead of hardcoding dependencies in your code, use dependency injection to provide the required dependencies dynamically.

---

By adhering to these principles, you can design systems that are easier to understand, modify, and extend over time. They form the bedrock of good object-oriented programming practices.
