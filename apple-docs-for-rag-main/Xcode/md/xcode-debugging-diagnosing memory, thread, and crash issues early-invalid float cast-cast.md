

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Invalid float cast 

Article

# Invalid float cast

Detects out-of-range casts to, from, or between floating-point types.

## Overview

Use this check to detect out-of-range casts to, from, or between floating-point types. Invalid casts have undefined behavior, and typically yield arbitrary values. These values may differ from platform to platform. Available in Xcode 9 and later.

### Invalid assignment of a double to a float in C

The cast from `n` to `m` results in undefined behavior because the destination type can’t represent its value.

```
double n = 10e50;
float m = (float)n; // Error: 10e50 can't be represented as a float.
```

#### Solution

Use a different destination type or avoid the cast altogether.

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

Invalid variable-length array

Detects negative array bounds.

