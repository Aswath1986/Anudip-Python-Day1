# Anudip-Python-Day1
Day 1 deliverables on Python learning

## Introduction to First Principles

Day 1 starts from how a machine sees the world and builds up to Python, one layer at a time.

### Repository contents

| File | What it is |
|------|------------|
| [Week1_Week_2_Python_Learning_Map_A3.pdf](Week1_Week_2_Python_Learning_Map_A3.pdf) | Week 1 and Week 2 Python learning map (A3) |
| [Human_Unlearning_Relearning_Python_First_Principles.jpeg](Human_Unlearning_Relearning_Python_First_Principles.jpeg) | First principles map, human version |
| [AI_Version_Unlearning_Relearning_Python_First_Principles.jpeg](AI_Version_Unlearning_Relearning_Python_First_Principles.jpeg) | First principles map, AI version |
| [Python_Hand_Written.jpeg](Python_Hand_Written.jpeg) | Handwritten Python notes |
| [Git_Project1_Local_Folder_to_GitHub.md](Git_Project1_Local_Folder_to_GitHub.md) | Git guide: push a local folder to GitHub |
| [Git_Project2_Fork_and_Add_Your_Files.md](Git_Project2_Fork_and_Add_Your_Files.md) | Git guide: fork a repo and add your files |

---

## Day 1 Concepts

### Framing strip: the machine world

- The machine world runs on **binary**
- **Bits and bytes**: a bit is 0 or 1; a byte is 8 bits
- **Encoding and decoding**: turning human data into bytes and back again
- The **interpreter** translates between our code and the machine
- Humans use **language** and **decimal**; machines use binary
- Numbers, alphabets, special characters, images, video and audio all become **bytes**
- Programs **read and write** to each other
- **Quantum computing and qubits** are the next frontier

### Phase 1: Foundations

- Python is a **high-level, interpreted, general-purpose** language
- Execution path: source `.py` → **bytecode** → **Python Virtual Machine (PVM)**
- **CPython** is the reference implementation
- **Objects live on the heap** in RAM
- **Names only point to objects**; they do not hold the values themselves
- **Line-by-line interpretation**
- **Portable**, but slower than compiled languages
- Well suited to: AI/ML, data, web, automation, scripting
- Less suited to: low-level systems, 3D engines, CPU-heavy threads

### Phase 2: Core basics

- An **identifier** is the name of a place in memory
- **Variables**
- **Constants** by convention (Python does not enforce them)
- **PEP 8** style guide and naming conventions:
  - `snake_case` for variables and functions
  - `UPPER_CASE` for constants
  - `PascalCase` for classes
  - `camelCase` (seen in other languages; not the Python convention)
- **Identifier rules**:
  - Letters, digits and underscore only
  - Cannot start with a digit
  - Case sensitive
  - Cannot be a keyword
- `#` **comments**
- **Docstrings** (`"""..."""`)
- `print()` for output
- `input()` for input (always returns a `str`)

### Phase 3: Data types, sequences, casting

| Category | Types | Mutability |
|----------|-------|------------|
| Numbers and boolean | `int`, `float`, `complex`, `bool` | Immutable |
| Collections | `list`, `set`, `dict`, `bytearray` | Mutable |
| Sequences and sets | `tuple`, `frozenset`, `range`, `str`, `bytes` | Immutable |
| Special | `NoneType`, `memoryview` | — |

- **Indexing**: `s[0]` (first), `s[-1]` (last)
- **Slicing**: `s[1:4]`
- **Reverse**: `s[::-1]`
- `len()` gives the length
- `in` checks membership
- **Mutable** objects change in place; **immutable** operations return a new object
- **Casting** with `int()`, `float()`, `str()`, `bool()`, `list()`, `tuple()`, `set()`, `dict()`
- Media as data:
  - An **image** is 3D bytes (height × width × channels)
  - A **video** is 4D (frames × height × width × channels)
  - **Audio** is a series of samples

### Phase 3+: Operators

- **Arithmetic**: `+ - * / // % **`
- **Assignment**: `= += -= *= /=` …, including the walrus operator `:=`
- **Relational**: `== != < > <= >=`
- **Logical**: `and or not`
- **Bitwise**: `& | ^ ~ << >>`
- **Membership**: `in`, `not in`
- **Identity**: `is`, `is not`
- An **expression** evaluates to a value; a **condition** evaluates to `True` or `False`

### Phase 4: Control flow and flow disruptors

- **Decisions**: `if` / `elif` / `else`, `match` / `case`
- **Loops**: `for`, `while`
- **Flow disruptors**: `break`, `continue`, `pass`, `return`, `yield`
- **Exception handling**: `try` / `except` / `else` / `finally`

### Parallel tracks

- **Errors**: syntax, runtime, logical and boundary errors
- **Reading tracebacks**
- **Testing**: `assert`, unit tests, integration tests
- **I/O**: user I/O, file I/O, JSON, database
- **Capstone project** that grows each phase

### Git guides

**Project 1: local folder to GitHub** ([guide](Git_Project1_Local_Folder_to_GitHub.md))

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git init
git status
git add .
git commit -m "First commit"
git branch -M main
git remote add origin <repo-url>
git push -u origin main
```

**Project 2: fork and contribute** ([guide](Git_Project2_Fork_and_Add_Your_Files.md))

- **Fork** the repository on GitHub
- **Clone** your fork: `git clone <your-fork-url>`
- Add the **upstream remote**: `git remote add upstream <original-repo-url>`
- Create a branch: `git checkout -b <branch-name>`
- Add, commit and push your files
- Open a **pull request**
