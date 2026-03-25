# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
from abc import ABC, abstractmethod
import math

# Abstract class
class Shape(ABC):
    
    @abstractmethod
    def calculate_area(self):
        pass


# Subclass 1
class Rectangle(Shape):
    
    def __init__(self, length, width):
        self.length = length
        self.width = width
    
    def calculate_area(self):
        return self.length * self.width


# Subclass 2
class Circle(Shape):
    
    def __init__(self, radius):
        self.radius = radius
    
    def calculate_area(self):
        return math.pi * self.radius ** 2

print("Rectangle Area")
l = float(input("Enter length: "))
w = float(input("Enter width: "))
rect = Rectangle(l, w)
print("Area of Rectangle:", rect.calculate_area())

print("\nCircle Area")
r = float(input("Enter radius: "))
circ = Circle(r)
print("Area of Circle:", circ.calculate_area())
## Output
<img width="430" height="344" alt="image" src="https://github.com/user-attachments/assets/2b0cb784-b137-4961-b4a5-f8833f39818d" />

## Result
Thus,the program was implemented and executed successfully,and the required output was obtained.
