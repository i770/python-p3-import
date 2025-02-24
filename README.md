# Python Imports Demonstration

This project demonstrates both absolute and relative imports in Python.

## Absolute Imports

```python
from lib.absolute_package.package1.module1 import function1
from lib.absolute_package.package2.subpackage1.module6 import function1 as function1_module6

function1()  # Output: Function 1 in module 1
function1_module6()  # Output: Function 1 in module 6
```

## Relative Imports

```python
# In lib/relative_package/subpackage1/subpackage2/module2.py
from .module1 import function1
from .. import module3

function1()  # Output: Function 1 from module1
module3.function1()  # Output: Function 1 from module3
```

## Running the Examples

1. For absolute imports:
   ```bash
   python test_absolute_imports.py
   ```

2. For relative imports:
   ```bash
   python -m lib.relative_package.subpackage1.subpackage2.module2
   ```

## Key Vocab

- **Module**: a file containing Python definitions and statements
- **Absolute Import**: Specifies the full path from the project root directory
- **Relative Import**: Uses dots to indicate the relative position in the package hierarchy
