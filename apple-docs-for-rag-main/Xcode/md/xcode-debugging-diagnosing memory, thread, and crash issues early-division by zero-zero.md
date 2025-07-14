

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Division by zero 

Article

# Division by zero

Detects division where the divisor is zero.

## Overview

Use this check to detect integer and float division where the divisor is zero. Division by zero has undefined behavior, and can result in crashes or incorrect program output. Available in Xcode 9 and later.

### Integer division by zero in C

In the following code, the `for` loop performs division by zero on its first iteration:

```
int sum = 10;
for (int i = 0; i 

Note

The optimizer may remove parts of a loop if it determines that undefined behavior might trigger in any of its iterations.

#### Solution

Modify the logic to check for and avoid division when the divisor might equal zero.

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

