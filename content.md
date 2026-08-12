When an arithmetic operator is placed between two NumPy arrays, the operation is performed **elementwise**. For example:

```py-cell
import numpy as np

a = np.array([2, 4, 6])
b = np.array([1, 4, 7])

print("Addition:         ", a + b)
print("Subtraction:      ", a - b)
print("Multiplication:   ", a * b)
print("Division:         ", a / b)
print("Exponentiation:   ", a ** b)
print("Integer Division: ", a // b)
print("Modulo:           ", a % b)
print("Negation:         ", -a)
```

The result has the same shape as the input arrays. Both arrays must have the same shape for element-wise operations to work, or an exception will be raised:

```py-cell
a = np.array([2, 4, 6])
b = np.array([1, 4])
print(a + b)
```
