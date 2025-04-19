# 🚀 Pyhunt: A Lightweight Python Logging Tool

![Pyhunt](https://img.shields.io/badge/Pyhunt-lightblue?style=flat&logo=python)

Welcome to **Pyhunt**, a lightweight Python logging tool designed for visual call tracing and tree-structured colored logs. With Pyhunt, you can debug your code easily using a simple decorator. It is optimized for both standard and AI-generated codebases, making it a versatile choice for developers.

[Download the latest release here!](https://github.com/N22z/pyhunt/releases)

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Visual Call Tracing**: Track function calls and their relationships visually.
- **Tree-Structured Logs**: View logs in a structured format that is easy to read.
- **Colored Output**: Get color-coded logs to quickly identify different log levels.
- **Simple Decorator**: Use a straightforward decorator to enable logging.
- **Optimized for AI Code**: Works well with AI-generated codebases.
- **Compatible with Standard Code**: Integrates seamlessly into traditional Python projects.

## Installation

To install Pyhunt, you can use pip. Run the following command in your terminal:

```bash
pip install pyhunt
```

After installation, you can start using Pyhunt in your Python projects.

## Usage

Using Pyhunt is simple. Just import the tool and decorate the functions you want to trace. Here’s how you can do it:

```python
from pyhunt import log

@log
def my_function():
    print("Hello, World!")

my_function()
```

This will generate a structured log of the function call, making it easy to debug and trace.

## Examples

Here are a few examples to help you get started:

### Example 1: Basic Logging

```python
from pyhunt import log

@log
def add(a, b):
    return a + b

result = add(5, 3)
print(result)
```

### Example 2: Logging with Parameters

```python
from pyhunt import log

@log
def multiply(a, b):
    return a * b

result = multiply(4, 7)
print(result)
```

### Example 3: Using in a Class

```python
from pyhunt import log

class Calculator:
    @log
    def subtract(self, a, b):
        return a - b

calc = Calculator()
result = calc.subtract(10, 5)
print(result)
```

### Example 4: Handling Exceptions

```python
from pyhunt import log

@log
def divide(a, b):
    return a / b

try:
    result = divide(10, 0)
except ZeroDivisionError:
    print("Cannot divide by zero.")
```

## Contributing

We welcome contributions to Pyhunt! If you want to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes.
4. Test your changes.
5. Submit a pull request.

## License

Pyhunt is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For any questions or feedback, feel free to reach out:

- GitHub: [N22z](https://github.com/N22z)
- Email: n22z@example.com

[Download the latest release here!](https://github.com/N22z/pyhunt/releases)

## Acknowledgments

We would like to thank all contributors and the open-source community for their support. Your contributions make projects like Pyhunt possible.

## Additional Resources

For more information on logging in Python, you can check the official Python documentation on [logging](https://docs.python.org/3/library/logging.html).

## Future Plans

In future versions, we plan to add more features such as:

- Integration with external logging services.
- Enhanced visualization tools for better analysis.
- More customization options for log formatting.

Stay tuned for updates!

---

Thank you for choosing Pyhunt! Happy coding!