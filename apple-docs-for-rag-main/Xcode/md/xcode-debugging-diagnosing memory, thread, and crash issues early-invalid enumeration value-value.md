

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Invalid enumeration value 

Article

# Invalid enumeration value

Detects when an enumeration variable has an invalid value.

## Overview

In Xcode 9 and later, you can use this check to detect accesses of an enumeration variable when its value isn’t within the valid range for the type. This can occur for uninitialized enumeration values, or when using an integer as an enumeration value without an appropriate cast. The use of out-of-range enumeration values has undefined behavior, and may indicate the existence of logic errors in a program.

### Invalid enumeration variable access in C++

In the following example, the cast to the `E` type is invalid because `2` isn’t within the enumeration’s range:

```
enum E {
    a = 1
};
int value = 2;
enum E *e = (enum E *)&value;
return *e; // Error: 2 is out of the valid range for E
```

#### Solution

Ensure that enumeration variables only use values within their defined ranges.

## See Also

### Undefined Behavior Sanitizer

Misaligned pointer

Detects when code accesses a misaligned pointer or creates a misaligned reference.

Invalid Boolean value

Detects when a program accesses a Boolean variable and its value isn’t true or false.

Out-of-bounds array access

Detects out-of-bounds access of arrays.

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

Invalid variable-length array

Detects negative array bounds.

