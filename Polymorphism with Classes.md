# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

---

## 💻 Program
class Beans:
    def type(self):
        print("Vegetable")

    def color(self):
        print("Green")

class Mango:
    def type(self):
        print("Fruit")

    def color(self):
        print("Yellow")

def show_info(obj):
    obj.type()
    obj.color()


b = Beans()
m = Mango()

show_info(b)
show_info(m)
## Output
<img width="343" height="235" alt="image" src="https://github.com/user-attachments/assets/5724560d-f99c-4016-91f6-a9b9070569bc" />

## Result
Thus,the program was implemented and executed successfully,and the required output was obtained.
