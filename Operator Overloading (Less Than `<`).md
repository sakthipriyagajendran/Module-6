# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program
class Number:
    
    def __init__(self, value):
        self.value = value
    
    # Overloading < operator
    def __lt__(self, other):
        return self.value < other.value

n1 = Number(10)
n2 = Number(20)
if n1 < n2:
    print("n1 is less than n2")
else:
    print("n1 is not less than n2")
## Output
<img width="371" height="209" alt="image" src="https://github.com/user-attachments/assets/9bed6239-d328-4c37-b507-38317de2a697" />

## Result
Thus,the program was implemented and executed successfully,and the required output was obtained.
