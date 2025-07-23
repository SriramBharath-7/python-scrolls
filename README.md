<p align="center">
  <img src="./visuals/Hello.gif" alt="Python Coding" width="600"/>
</p> <br></br>

<details>
  <summary>📂 Python Basics Cheatsheet </summary> <br></br>

# 🐍 Python Basics Cheatsheet 
> 🚀 Master the essentials of Python – your gateway to automation, web dev, data science, and beyond.

---

## 🧠 Python Syntax Overview

```python
# This is a comment
# (Think of this like a note for humans, Python ignores it)

print("Hello, world!")  # Output something to the screen
# This shows the words “Hello, world!” on your screen
```

---

## 🔢 Variables and Data Types

Variables are like boxes where you can store stuff — numbers, words, or True/False.

```python
# Numbers
x = 10          # x is a box that holds the number 10 (integer)
pi = 3.14       # pi holds a decimal number (called a float)

# Strings (words inside quotes)
name = "Sri"    # name holds the word Sri
greeting = 'Hello'  # greeting holds Hello (single or double quotes both work)

# Booleans (True or False — like Yes or No)
is_coding = True     # means YES, I am coding
is_sleeping = False  # means NO, I am not sleeping
```

---

## 🎯 Input and Output

Input lets you *ask* the user something. Output shows something on the screen.

```python
name = input("What's your name? ")
# This asks the user their name and saves it into a box called 'name'

print("Hello", name)
# This shows: Hello <whatever the user typed>
```

🧸 Example:
```
What's your name? → Sri  
Output: Hello Sri
```

---

## 🧮 Operators

Operators help us **do things** like math, comparisons, and logic.

```python
# Arithmetic Operators (like in school)
+  # Add things
-  # Subtract
*  # Multiply
/  # Divide
%  # Remainder after division
** # Power (2 ** 3 means 2 to the power of 3 = 8)
// # Floor divide (cuts off decimals)

# Comparison Operators
==  # Is equal to?
!=  # Is NOT equal?
>   # Greater than?
<   # Less than?
>=  # Greater than or equal to?
<=  # Less than or equal to?

# Logical Operators
and  # Both conditions must be True
or   # At least one must be True
not  # Opposite of the condition
```

🧸 Example:
```python
2 + 3 == 5  # True
5 > 3 and 2 < 4  # True
not True  # False
```

---

## 🔁 Control Flow

Control flow means **making decisions** and **repeating stuff**.

### ✅ Conditional Statements:

```python
if x > 0:
    print("Positive")
elif x == 0:
    print("Zero")
else:
    print("Negative")
```

🧸 Example:
If `x = 5`, it prints “Positive”.  
If `x = 0`, it prints “Zero”.

---

### 🔄 Loops:

Loops repeat things over and over.

```python
# For loop: Repeat a fixed number of times
for i in range(5):
    print(i)
```

🧸 Output:
```
0
1
2
3
4
```

```python
# While loop: Keep going until something is False
count = 0
while count < 5:
    print(count)
    count += 1  # Adds 1 each time
```

🧸 Output:
```
0
1
2
3
4
```

---

## 📦 Functions

Functions are like mini-machines. You give them input, they give you output.

```python
def greet(name):
    return "Hello " + name

message = greet("Sri")
print(message)
```

🧸 Output:
```
Hello Sri
```

Explanation:
- `def greet(name):` creates a function named `greet`
- `return` gives back the result
- You can reuse the function as many times as you want!

---

## 📚 Lists and Loops

Lists are like toy boxes that hold multiple items.

```python
fruits = ["apple", "banana", "cherry"]
# A list of 3 fruits

for fruit in fruits:
    print(fruit)  # Print each fruit one by one
```

🧸 Output:
```
apple
banana
cherry
```

```python
fruits.append("mango")  # Add mango to the list

print(fruits[0])  # Shows the first fruit: apple
```

---

## 🧰 Common Built-in Functions

Python has lots of ready-made tools (functions) you can use:

```python
len("hello")      # Gives 5 (the number of letters)
type(10)          # Says it's an int (number)
int("5")          # Turns the string "5" into a number
str(10)           # Turns number 10 into a string
float("3.14")     # Makes it a decimal number
bool("")          # Empty things are False, others are True
range(3)          # Makes numbers 0, 1, 2
```

🧸 Example:
```python
list(range(3)) → [0, 1, 2]
```

---

## 💡 Tips

- Use `snake_case` for variable and function names (like: `total_score`, `get_input`)
- Indentation (spacing) is VERY important! Always use 4 spaces.
- To run your Python file:
  ```bash
  python filename.py
  ```

---

  </details>



<details>
  <summary>📂 Python Data Structures Cheatsheet </summary> <br></br>

  # 🧱 Python Data Structures Cheatsheet 



> 🎯 Data structures let you store, access, and organize your stuff (like toys, lists, or cards).  
> They help you **remember things, find them fast, and keep them tidy** when you're coding!

---

## 🧺 1. Lists (A basket that holds items in order — and you can change them!)

```python
fruits = ["apple", "banana", "mango"]
```

🧸 This is a **list** — like a toy basket.  
It has three fruits, and you can do lots of things with it:

```python
fruits.append("orange")     # Adds "orange" to the basket
fruits.remove("banana")     # Takes "banana" out
fruits[0]                   # Gets the first fruit ("apple")
fruits[1] = "grape"         # Changes second fruit to "grape"
len(fruits)                 # Counts how many fruits are in the basket
```

### 🔁 Loop through list (Look at each item one by one)

```python
for fruit in fruits:
    print(fruit)
```

🧸 This prints each fruit one by one like:
```
apple  
grape  
mango  
orange  
```

---

## 📚 2. Tuples (A list you can't change — like a locked box)

```python
coordinates = (10, 20)
print(coordinates[0])     # Gets the first number (10)
```

🧸 Tuples are like **coordinates** on a map.  
You can look at them, but **you can't change them**.

🔒 Use tuples when your data should stay the same.  
Example: `(latitude, longitude)`, or sizes like `(width, height)`

---

## 🗃️ 3. Dictionaries (A label-sticker box: each item has a name and a value)

```python
person = {"name": "Sri", "age": 17}
```

🧸 This is a dictionary. It’s like a **box where each item has a label**:

```python
print(person["name"])        # Shows "Sri"
person["age"] = 18           # Changes age to 18
person["city"] = "Chennai"   # Adds a new label: "city"
```

### 🔁 Loop through dictionary (Check all labels and values)

```python
for key, value in person.items():
    print(key, value)
```

🧸 Output:
```
name Sri  
age 18  
city Chennai
```

---

## 🔢 4. Sets (A magic bag with only unique things – no duplicates allowed!)

```python
numbers = {1, 2, 3, 2, 1}
```

🧸 This bag only keeps **one of each number**, so it becomes:
```
{1, 2, 3}
```

```python
numbers.add(4)        # Adds number 4
numbers.remove(2)     # Removes number 2
```

👀 You can also **check if something’s in the set**:

```python
if 3 in numbers:
    print("Found")
```

🧸 Output:
```
Found
```

---

## 📊 Summary Table

| Type        | Ordered | Can Change? | Allows Duplicates? | Example            |
|-------------|---------|-------------|---------------------|--------------------|
| **List**     | ✅ Yes  | ✅ Yes      | ✅ Yes              | `["a", "b", "c"]`  |
| **Tuple**    | ✅ Yes  | ❌ No       | ✅ Yes              | `(1, 2, 3)`        |
| **Dictionary** | ✅ Yes (by key) | ✅ Yes | ❌ No (keys must be unique) | `{"key": "value"}` |
| **Set**      | ❌ No   | ✅ Yes      | ❌ No               | `{1, 2, 3}`        |

---

## 🧠 Pro Tips

- ✅ Use **lists** when you need an **ordered group** of things you want to **change**
- 🔒 Use **tuples** when the data should **never change**
- 🏷️ Use **dictionaries** when each value needs a **name or label**
- 🧹 Use **sets** to **remove duplicates** or **check if something exists**

---

</details>

