# 03c - Sets (Data Structures)

## 📅 Date

Completed: 17/06/2026

## 📚 Topics Covered

- Creating and accessing sets
- Adding and removing elements
- Set operations: union, intersection, difference, symmetric difference
- Set comprehensions
- Filtering sets
- Removing duplicates using sets
- Subsets and supersets
- Frozensets
- Converting between sets and lists
- Sets as dictionary keys (via frozenset)
- Iterating over sets
- Removing elements until empty
- Symmetric difference update
- Set membership testing
- Set of tuples

## 🧠 What I Learned

- **No duplicates, no order:** A set automatically drops duplicate values and doesn't preserve the order items were added in — very different from lists and tuples.
- **Set operations mirror math:** `|` (union), `&` (intersection), `-` (difference), and `^` (symmetric difference) work just like the set operations from math class.
- **Frozenset:** An immutable version of a set — same relationship as tuple is to list. Needed whenever a set-like value has to stay fixed (e.g. as a dictionary key).
- **Sets can't be dictionary keys, but frozensets can:** Regular sets are mutable, so Python won't allow them as dictionary keys. Frozensets are immutable, so they work — this connected directly back to what I learned about tuples being hashable.
- **Membership testing (`in`) is fast on sets:** Checking if something exists in a set is much more efficient than doing the same check on a list, especially for large collections.
- **`.pop()` on a set removes a random element** — not the first one, since sets have no defined order (unlike list `.pop()` which removes the last item).

## 💡 Key Takeaways

Sets clicked quickly because I'd already seen the "immutable vs mutable" pattern with tuples and lists — frozenset just applies that same idea to sets. The most useful realization was _why_ sets exist: when you don't care about order or duplicates and just want to answer "what's here" or "what overlaps between these two groups," a set is the right tool. The dictionary key restriction (Assignment 10) was the best learning moment — it wasn't just a rule to memorize, it made me actually understand hashability instead of just tuples "being allowed" as keys.

## 🚧 Challenges

- Getting used to sets having no guaranteed order took adjustment — printing a set doesn't always show elements in the order they were added.
- Understanding _why_ Assignment 10 fails with a regular set (and why frozenset fixes it) required connecting it back to the tuple lesson on immutability/hashability.
- Remembering the difference between `^` (symmetric difference, creates new set) and `.symmetric_difference_update()` (changes the set in place) took a couple of tries to keep straight.

## 🔗 Files in this folder

- `sets_assignment.ipynb` — 15 solved exercises covering set creation, operations, comprehensions, and conversions
