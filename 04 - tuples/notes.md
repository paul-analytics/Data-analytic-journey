# 03b - Tuples (Data Structures)

## 📅 Date

Completed: 14/07/2026

## 📚 Topics Covered

- Creating and accessing tuples
- Indexing (first, middle, last elements)
- Tuple slicing
- Nested tuples (matrices)
- Tuple concatenation
- Tuple methods (`count`, `index`)
- Unpacking tuples
- Converting between tuples and lists
- Tuple of tuples
- Tuples and strings
- Tuples as dictionary keys
- Nested tuple iteration
- Converting tuples to sets
- Writing functions that operate on tuples (min, max, sum)

## 🧠 What I Learned

- **Tuples vs lists:** Tuples look and behave like lists (ordered, indexable, sliceable) but are **immutable** — once created, they can't be changed. This makes them useful for data that should stay fixed/protected from accidental edits.
- **Limited methods:** Unlike lists, tuples only have two built-in methods — `.count()` and `.index()` — a direct result of not being editable.
- **Unpacking:** Tuples can be "unpacked" directly into separate variables in one line (e.g. `a, b, c = my_tuple`), which is a clean way to pull out multiple values at once.
- **Editing a tuple indirectly:** Since tuples can't be modified directly, the workaround is: convert to a list → make changes → convert back to a tuple.
- **Tuples as dictionary keys:** Because tuples are immutable, they can be used as dictionary keys — something lists can never do, since dictionary keys must never change.
- **Converting to a set:** Turning a tuple into a `set()` is a fast way to remove duplicate values, same trick used with lists.

## 💡 Key Takeaways

This lesson built directly on the Lists module, which made it easier to pick up — most operations (indexing, slicing, nesting, iterating) work the same way. The real "aha" moment was understanding _why_ tuples exist at all: immutability isn't a limitation, it's intentional — useful for fixed data (like coordinates, or dictionary keys) where you want to guarantee nothing changes by accident. Seeing tuples used as dictionary keys was a good example of a real use case that lists simply can't do.

## 🚧 Challenges

- Initially wasn't clear why tuples would ever be preferred over lists, since lists seem more flexible — understanding the immutability use case took some thought.
- The list → tuple → list conversion workaround for "editing" a tuple felt clunky at first, but makes sense once you understand tuples are meant to be fixed.
- Remembering that tuples only have `.count()` and `.index()` (not the wide range of list methods) took a moment to adjust to.

## 🔗 Files in this folder

- `tuple_assignment.ipynb` — 15 solved exercises covering tuple creation, slicing, unpacking, conversions, and tuple-based functions
