

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Invalid variable-length array 

Article

# Invalid variable-length array

Detects negative array bounds.

## Overview

Use this check to detect negative array bounds. Variable-length arrays with a negative length have undefined behavior, and may cause stack corruption. Available in Xcode 9 and later.

### Negative variable-length array bounds in C

In the following code, the call to the `invalid_index_returning_function` function returns a negative number that results in an invalid array:

```
int invalid_index_returning_function() {
    return -1;
}
int idx = invalid_index_returning_function();
int array[idx]; // Error: invalid array length
```

#### Solution

Fix the issue by checking array bounds before constructing arrays.

## See Also

### Undefined Behavior Sanitizer

Misaligned pointer

Detects when code accesses a misaligned pointer or creates a misaligned reference.

Invalid Boolean value

Detects when a program accesses a Boolean variable and its value isn’t true or false.

Out-of-bounds array access

Detects out-of-bounds access of arrays.

Invalid enumeration value

Detects when an enumeration variable has an invalid value.

Reaching of unreachable point

Detects when a program reaches an unreachable point.

Dynamic type violation

Detects when an object has the wrong dynamic type.

Invalid float cast

Detects out-of-range casts to, from, or between floating-point types.

Division by zero

Detects division where the divisor is zero.

Nonnull argument violation

Detects when an argument incorrectly receives a null value.

Nonnull return value violation

Detects when a function incorrectly returns null.

Nonnull variable assignment violation

Detects when you incorrectly assign null to a variable.

Null reference creation and null pointer dereference

Detects the creation of null references and null pointer dereferences.

Invalid object size

Detects invalid pointer casts due to differences in the sizes of types.

Invalid shift

Detects invalid and overflowing shifts.

Integer overflow

Detects overflow in arithmetic.

