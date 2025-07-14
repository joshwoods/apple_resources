

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Reaching of unreachable point 

Article

# Reaching of unreachable point

Detects when a program reaches an unreachable point.

## Overview

Use this check to detect when control flow reaches an unreachable point in a program you create using `__builtin_unreachable`, which may cause abrupt program termination. Available in Xcode 9 and later.

### Executing unreachable code in C

If the `switch` statement fails to handle a value that a function returns, the program reaches `__builtin_unreachable()`.

```
switch (value_returning_function()) {
case ...:                  // Warning: if the cases are not exhaustive
default:                   // __builtin_unreachable may be reached
    __builtin_unreachable();
}
```

#### Solution

Ensure that `switch` statements and other control flow statements are exhaustive.

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

Invalid variable-length array

Detects negative array bounds.

