# Python — Files, Parsing, CLI

Three small exercises practicing file I/O, regex, `pathlib`, and a basic command-line dispatcher.

## Stack

- Python 3.12 (standard library only)

## Exercises

### `hw4_1.py` — salary file parser

`total_salary(path)` reads a text file where each line is `Last_Name,salary` and returns `(total, average)` over all rows. Returns `(0, 0)` and prints a message on bad paths or malformed input.

### `hw4_2.py` — cats CSV parser

`get_cats_info(path)` reads a CSV with `id,name,age` per line and returns a list of dicts:

```python
[{"id": "60b90c1c13067a15887e1ae1", "name": "Tayson", "age": "3"}, ...]
```

Returns `None` on path errors or rows that don't have exactly three fields.

### `hw4_4.py` — contact CLI

A simple in-memory contact dispatcher with these commands:

| Command | Action |
|---------|--------|
| `add <name> <phone>` | Create a contact |
| `change <name> <phone>` | Update a phone |
| `phone <name>` | Show one contact |
| `all` | Show every contact |
| `hello` | Greeting |
| `close` / `exit` | Quit |

`parse_input` splits the user's line; each handler returns a string that the main loop prints.

## Run

```bash
python hw4_1.py
python hw4_2.py
python hw4_4.py
```
