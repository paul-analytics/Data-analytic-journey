# 03 - Lists (Data Structures)

## 📅 Date

Completed: 14/07/2026

## 📚 Topics Covered

- Creating and accessing lists
- Indexing (first, middle, last elements)
- List slicing
- List comprehensions
- Filtering lists with comprehensions
- List methods (sorting, removing duplicates)
- Nested lists (matrices)
- List of dictionaries
- Matrix transposition
- Flattening nested lists
- List manipulation (insert/delete by index)
- Zipping lists together
- List reversal
- List rotation
- List intersection

## 🧠 What I Learned

- **Indexing:** Lists start counting at 0, not 1 — so the "first" item is `list[0]`. Negative indexing (`list[-1]`) is a shortcut for counting from the end.
- **Slicing:** `list[start:end]` grabs a chunk of the list — the end position is never included, which took some getting used to.
- **List comprehensions:** A one-line shortcut for building a new list from a rule (e.g. `[x**2 for x in range(1,11)]`), instead of writing a full loop with `.append()`. Can also include an `if` condition to filter as you build.
- **Nested lists:** A "list of lists" is how you represent a grid or matrix — accessing an element means indexing twice (`matrix[row][col]`).
- **List of dictionaries:** Similar to rows in a spreadsheet — each dictionary is a record with labeled fields (`key: value`), and a list of them can be sorted by a specific field using `sorted(..., key=...)`.
- **set() for duplicates:** Since sets can't hold repeated values, converting a list to a set (then back to a list) is a fast way to remove duplicates.
- **zip():** Pairs up two lists item-by-item into tuples — useful for combining related data (like names and their scores).
- **Modifying lists safely:** When deleting multiple items by index, deleting from the highest index first avoids accidentally shifting and breaking the remaining indices.

## 💡 Key Takeaways

This module felt like a big jump from Module 2 — lists are the first real "data structure," and a lot of what's coming in data analytics (tables, rows, columns) builds directly on this. List comprehensions were the most valuable new tool: once it clicked, it replaced a lot of clunky loop-and-append code with a single readable line. Nested lists and list-of-dictionaries also made it clear how Python can represent more complex, real-world data (like a spreadsheet or a matrix) using just lists.

## 🚧 Challenges

- List comprehensions were confusing at first — reading them left to right as "give me X, for every item, if condition" took a few tries to get comfortable with.
- Slicing off-by-one mistakes were common early on — forgetting that the end index isn't included in the result.
- Understanding nested list indexing (`matrix[row][col]`) took a moment to visualize — had to slow down and think of it as "pick the row first, then pick the item inside that row."
- Deleting multiple list items by index without breaking the remaining indices required extra care — learned to delete from the back of the list first.

## 🔗 Files in this folder

- `list_Assignment.ipynb` — 15 solved exercises covering list creation, slicing, comprehensions, nested lists, and list operations
