# 3.4 - Dictionaries (Data Structures)

## 📅 Date
Completed: 23/07/2026

## 📚 Topics Covered
- Creating and accessing dictionaries
- Dictionary methods (add, remove/pop)
- Iterating over dictionaries
- Dictionary comprehensions
- Merging dictionaries
- Nested dictionaries
- Dictionary of lists / dictionary of tuples
- Converting dictionaries to lists of tuples
- Filtering dictionaries
- Swapping keys and values
- Default dictionaries (`defaultdict`)
- Counting with dictionaries
- Converting dictionaries to JSON

## 🧠 What I Learned
- **Key-value pairs:** Unlike lists/tuples/sets which store single values, dictionaries store labeled data — you look things up by key instead of position, like `d[5]` instead of `d[0]`.
- **Dictionary comprehensions:** Same shortcut pattern as list/set comprehensions, just building `key: value` pairs in one line (e.g. `{i: i**2 for i in range(1, 11)}`).
- **`.items()` is the key to iterating:** Looping with `.items()` gives both the key and value together, which is what you almost always want when going through a dictionary.
- **`.update()` merges dictionaries** — combining two dictionaries into one by adding all of the second dictionary's pairs into the first.
- **Nested dictionaries:** A dictionary can hold another dictionary as a value — useful for representing structured, real-world data (like a student record with a nested grades dictionary).
- **`.get(key, default)`** is a safe way to look up a value without crashing if the key doesn't exist yet — this is what makes the character-counting function work cleanly.
- **`defaultdict`:** Automatically creates a default value (like an empty list) for any new key the first time it's touched, avoiding manual key-existence checks.
- **JSON connection:** A Python dictionary converts almost directly into JSON format using `json.dumps()` — this is the same format used for APIs and web data, so dictionaries are the bridge between Python and that outside world.

## 💡 Key Takeaways
Dictionaries felt like the most "practical" data structure so far — a lot of real data (student records, config settings, API responses) naturally maps to key-value pairs rather than plain ordered lists. The key/value swap exercise was a good reminder to think about data integrity (duplicate values would silently overwrite each other), and the JSON exercise made the connection between what I'm learning and how data actually moves between programs and the web. This module tied together everything from Lists, Tuples, and Sets — dictionaries can hold any of them as values, and tuples specifically work well as dictionary keys because they're immutable.

## 🚧 Challenges
- Remembering that dictionary keys must be unique and immutable (hashable) took some connecting back to what I learned with tuples and frozensets.
- The key/value swap (Assignment 12) made me realize duplicate values would cause data loss — something I hadn't thought about until I saw the mechanics of how the new dictionary gets built.
- `defaultdict` felt like "magic" at first — understanding that it just auto-fills a default value on first access (instead of raising a `KeyError`) took a moment to click.

## 🔗 Files in this folder
- `dictionaries_assignment_solution.ipynb` — 15 solved exercises covering dictionary creation, comprehensions, nesting, filtering, and JSON conversion
