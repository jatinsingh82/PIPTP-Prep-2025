def fun(w, x):
    y = 0
    if ((x % w == 0) or (w % x) == 0):
        y = y + 1
    else:
        y = y + 10
    print(y)

print(fun(40, 4))
🔹 Descriptive Solution:
Let's walk through the function fun(w, x) step by step for the input w = 40, x = 4:

The function starts by initializing y = 0.

The condition in the if statement is:

scss
Copy
Edit
(x % w == 0) or (w % x == 0)
Evaluate x % w == 0 → 4 % 40 = 4, which is not equal to 0 → False

Evaluate w % x == 0 → 40 % 4 = 0 → True

Since the condition uses or, and one part is True, the entire condition is True

Because the condition is True, it executes:

python
Copy
Edit
y = y + 1  # y becomes 1
It then prints y, which is 1.

Finally, the function ends. But note: there's no return statement in the function, so the function implicitly returns None.

🔹 Answer:
css
Copy
Edit
1
None
✅ Explanation:
1 is printed from inside the function using print(y)

None is printed by the outer print(fun(40, 4)), because the function does not return anything
