

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Nonnull variable assignment violation 

Article

# Nonnull variable assignment violation

Detects when you incorrectly assign null to a variable.

## Overview

Use this check to detect when you assign `null` to a variable with the `_Nonnull` annotation. Available in Xcode 9 and later.

Note

The nonnull violation check for variable assignment is off by default. You can turn it on by enabling the `-fsanitize=nullability-assign` compiler flag.

### Violation of nonnull annotation with variable assignment in C

In the following example, the call to `assigns_a_value` breaks the `_Nonnull` annotation of the variable `q`:

```
void assigns_a_value(int *p) {     
    int *_Nonnull q = p; // Warning: null can be assigned
}
assigns_a_value(NULL); // Error: _Nonnull variable violation
```

#### Solution

Correct logic errors, or remove the `_Nonnull` annotation.

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

