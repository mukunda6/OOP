# 📘 Object-Oriented Programming (OOP) Notes

## 🚀 Introduction
Object-Oriented Programming (OOP) is a programming paradigm based on the concept of **objects**, which contain data (attributes) and methods (functions).

OOP helps in:
- Code reusability
- Modularity
- Scalability
- Real-world modeling

---

# 🧱 4 Pillars of OOP

## 1️⃣ Encapsulation
Encapsulation means wrapping data and methods into a single unit (class) and restricting direct access.

### Example (Python):
```python
class Student:
    def __init__(self, name, marks):
        self.name = name
        self.__marks = marks   # private variable

    def get_marks(self):
        return self.__marks

s = Student("Mukunda", 95)
print(s.get_marks())
```

✅ Data is protected using private variables.

---

## 2️⃣ Abstraction
Abstraction means hiding internal implementation and showing only essential features.

### Example:
```python
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass
```

✅ User only knows that `area()` exists, not how it is implemented.

---

## 3️⃣ Inheritance
Inheritance allows one class to inherit properties and methods from another class.

### Example:
```python
class Animal:
    def sound(self):
        print("Animal makes sound")

class Dog(Animal):
    def bark(self):
        print("Dog barks")

d = Dog()
d.sound()
d.bark()
```

✅ Code reuse achieved.

---

## 4️⃣ Polymorphism
Polymorphism means same function name, different behavior.

### Example:
```python
class Cat:
    def sound(self):
        print("Meow")

class Dog:
    def sound(self):
        print("Bark")

for animal in [Cat(), Dog()]:
    animal.sound()
```

✅ Same method name, different outputs.

---

# 🔑 Important OOP Concepts

## ✔️ Class
Blueprint for creating objects.

## ✔️ Object
Instance of a class.

## ✔️ Constructor
Special method used to initialize objects.

## ✔️ Destructor
Used to clean up resources.

---

# 🎯 Advantages of OOP
- Code Reusability
- Data Security
- Easy Maintenance
- Better Structure
- Scalable Applications

---

# 📌 Real World Example
Bank Account System:
- Class: BankAccount
- Attributes: balance, account_number
- Methods: deposit(), withdraw()

---

# 🧠 Interview Important Questions

1. What are the 4 pillars of OOP?
2. Difference between abstraction and encapsulation?
3. What is method overloading?
4. What is method overriding?
5. What is the difference between class and object?
6. What is the difference between composition and inheritance?

---

# 🏁 Conclusion
OOP is essential for building scalable and maintainable software.  
Mastering OOP concepts is important for technical interviews and real-world development.

---

⭐ If you found this helpful, feel free to star this repository!
