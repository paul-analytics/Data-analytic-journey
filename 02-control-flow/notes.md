# 02 - Control Flow (Conditionals & Loops)

## 📅 Date

Completed: (11/07/2026)

## 📚 Topics Covered

- Conditional statements: `if`, `if-else`, `if-elif-else`, nested `if`
- Loops: `for` loop, `while` loop, nested loops
- Loop control: `break`, `continue`, `pass`
- Combining loops with conditionals
- Applied problems: factorial, sum of digits, prime check, Fibonacci sequence

## 🧠 What I Learned

- **Conditionals:** How to make a program branch and make decisions using `if`, `elif`, and `else`, including nesting one condition inside another.
- **for loop:** Best used when I know how many times to repeat something, or I'm looping through a list/range of numbers.
- **while loop:** Best used when the number of repeats depends on a condition rather than a fixed count — and why it's easy to accidentally create an infinite loop if the condition never changes.
- **break vs continue vs pass:**
  - `break` = exit the loop immediately
  - `continue` = skip this round, move to the next one
  - `pass` = do nothing (placeholder so Python doesn't error on empty code)
- **Nested loops:** A loop inside another loop — useful for grid/pattern problems like printing a 5x5 grid.
- **Modulo (`%`) and floor division (`//`):** Used together to break numbers apart digit by digit (e.g. sum of digits) or check divisibility (e.g. even numbers, prime checks).

## 💡 Key Takeaways

This module was about control — teaching the program to make decisions and repeat actions instead of just running top to bottom. The biggest shift from Module 1 was realizing that `for` and `while` solve different problems: `for` when I know the range, `while` when I'm watching for a condition to change. Working through problems like factorial, sum of digits, and prime checking helped me see how these tools combine in real logic, not just isolated examples.

## 🚧 Challenges

- Deciding between `for` and `while` for a given problem wasn't always obvious at first — I had to think about whether I knew the exact number of repeats.
- Nested loops (the 5x5 grid) took a moment to visualize — understanding that the outer loop controls rows and the inner loop controls columns.
- Using `break` inside a `while True` loop felt unusual at first, since the loop technically "never stops" on its own — the `break` is what's actually controlling it.
- Digit-by-digit problems (sum of digits) required combining `%` and `//` together, which took some trial and error to fully understand.

## 🔗 Files in this folder

- `assignments.py` — 15 solved exercises covering conditionals, loops, and loop control statements
