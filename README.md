# Basic Math Library

This package provides users with a basic interface for evaluating functions.

## Usage

```py
from symMath_adasneves127.equation import create_eq

eq = create_eq("5x^2 + 3x + 5")

eq.evaluate(4) # Evaluate the equation when x=4

eq.evaluate(7.21) # Evaluate the equation when x=7.21
```

The 'equation' function will prvide an object with the following methods for use:

* Print
* Evaluate
  
Print will print out how the program interpreted the equation given.

Evaluate takes in a parameter 'x', to be used as the variable placeholder.

---

## Implementation with matplotlib

```python
# Import the required libraries and functions
from symMath_adasneves127.equation import create_eq
from matplotlib import pyplot as plt

# Create a basic equation of x^2
equation = create_eq("x^2")


# Unfortunately, the 'Range' function does not support floating point step values.
x = -10
while x < 10:
    y = equation.evaluate(x) # Evaluate, plot, increment.
    plt.plot(x, y, 'ro')
    x += 0.1

# Show the plot
plt.show()

```

![Plot Result](./result.png)

If your program is working correctly, you should see something like the figure above.

## More info

[Github](https://github.com/adasneves127/mathSym)
