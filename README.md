# Pycyclic
Pycyclic is a python Library that helps you to developing any program like, core development, games development, etc...

Version: 0.1.0

## Features
- Rotate sequences left or right by a given number of steps
- Repeat sequences multiple times
- Create cyclic iterators
- Take n elements from a cyclic iterator
- Detect cycles in sequences
- Check if a sequence is cyclic
- Modular and easy-to-integrate UI

## Installation
You can install PyCyclic directly from PyPI:

```bash
pip install pycyclic
```
## Usage
Core Development example:
```python
from pycyclic.core import rotate, cyclic_iterator, take, repeat, find_cycle, is_cyclic

seq = [1, 2, 3, 4, 5]

# Rotate
print(rotate(seq, 2, direction="right"))  # [4, 5, 1, 2, 3]

# Cyclic Iterator
cyc = cyclic_iterator(seq)
print(take(7, cyc))  # [1, 2, 3, 4, 5, 1, 2]

# Repeat sequence
print(repeat(seq, 2))  # [1, 2, 3, 4, 5, 1, 2, 3, 4, 5]

# Find smallest cycle
print(find_cycle([1, 2, 3, 1, 2, 3]))  # [1, 2, 3]

# Check if cyclic
print(is_cyclic([1, 2, 3, 1, 2, 3]))  # True
```

UI Example:
```python
from pycyclic.ui import main

# Make a window
main.window("Example window")

# Messaging
show_msg(title, text, kind)
# |
# |
# v
show_msg("Error", "This is an error", "error")
show_msg("Info", "This is an Info", "info")
show_msg("Warning", "This is an warning", ""e)
```

## Contribution
Contributions are welcome! Feel free to open issues or submit pull requests for bug fixes and new features.

