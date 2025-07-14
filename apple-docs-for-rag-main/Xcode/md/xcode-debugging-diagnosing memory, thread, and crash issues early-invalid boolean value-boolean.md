

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Invalid Boolean value 

Article

# Invalid Boolean value

Detects when a program accesses a Boolean variable and its value isn’t true or false.

## Overview

Use this check to detect accesses to a Boolean variable when its value isn’t true or false. This problem can occur when using an integer or pointer without an appropriate cast. The use of out-of-range Boolean values has undefined behavior, which can be difficult to debug. Available in Xcode 9 and later.

### Invalid Boolean variable access in C

The intent of the following code is to call the `success` function when `result` is nonzero. However, because it uses a Boolean check, the compiler may, as an optimization, only emit instructions that check the least-significant bit of `predicate`, which is `0`, causing a logic error.

```
int result = 2;
bool *predicate = (bool *)&result;
if (*predicate) { // Error: variable is not a valid Boolean
    success();
}
```

#### Solution

Use integer comparison instead of a Boolean check.

```
int result = 2;
if (result != 0) { // Correct
  success();
}
```

## See Also

### Undefined Behavior Sanitizer

Misaligned pointer

Detects when code accesses a misaligned pointer or creates a misaligned reference.

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

Invalid variable-length array

Detects negative array bounds.

