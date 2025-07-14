

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Nonnull argument violation 

Article

# Nonnull argument violation

Detects when an argument incorrectly receives a null value.

## Overview

Use this check to detect when a function that has an argument with the `nonnull` attribute or the `_Nonnull` annotation receives a null value. Available in Xcode 9 and later.

Note

The nonnull violation check for arguments with the `_Nonnull` annotation is off by default. You can turn it on by enabling the `-fsanitize=nullability-arg` compiler flag.

### Violation of the nonnull parameter attribute in C

In the following example, the call to the `has_nonnull_argument` function breaks the `nonnull` attribute of the parameter `p`:

```
void has_nonnull_argument(__attribute__((nonnull)) int *p) { 
     // ... 
}
has_nonnull_argument(NULL); // Error: nonnull parameter attribute violation
```

#### Solution

Correct logic errors, or remove the `nonnull` attribute and rework the called function’s logic accordingly.

### Violation of the nonnull annotation for an argument in C

In the following example, the call to the `has_nonnull_argument` function breaks the `_Nonnull` annotation of the parameter `p`:

```
void has_nonnull_argument(int * _Nonnull p) { 
     // ... 
}
has_nonnull_argument(NULL); // Error: _Nonnull annotation violation
```

#### Solution

Correct logic errors, or remove the `_Nonnull` attribute and rework the called function’s logic accordingly.

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

