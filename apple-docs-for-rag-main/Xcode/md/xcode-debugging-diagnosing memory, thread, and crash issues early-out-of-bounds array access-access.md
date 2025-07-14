

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Out-of-bounds array access 

Article

# Out-of-bounds array access

Detects out-of-bounds access of arrays.

## Overview

Use this check to detect attempts to access indexes that exceed the array’s bounds. Out-of-bounds array accesses have undefined behavior, and can result in crashes or incorrect program output. Available in Xcode 9 and later.

Note

This check doesn’t detect out-of-bounds accesses into heap-allocated arrays.

### Out-of-bounds array access in C

In the following example, out-of-bounds access of `array` occurs on the last iteration of the loop:

```
int array[5];
for (int i = 0; i 

#### Solution

Ensure that accessed indexes don’t exceed the array’s bounds.

## See Also

### Undefined Behavior Sanitizer

Misaligned pointer

Detects when code accesses a misaligned pointer or creates a misaligned reference.

Invalid Boolean value

Detects when a program accesses a Boolean variable and its value isn’t true or false.

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

