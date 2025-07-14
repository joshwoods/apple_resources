

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Invalid shift 

Article

# Invalid shift

Detects invalid and overflowing shifts.

## Overview

Use this check to detect bitwise shifts with invalid shift amounts and shifts that might overflow. These shifts have undefined behavior and the optimizer may omit them. Available in Xcode 9 and later.

### Invalid shift amount in C

The following code shows a shift with an invalid shift amount because the destination type can’t represent the result:

```
int32_t x = 1;
x 

If the optimizer can prove that a shift amount may be invalid, it may replace the result of the shift with an arbitrary value.

#### Solution

Use a larger destination type, such as an `int64_t`.

### Shift overflow in C

In the following code, the second shift overflows `x` because `int32_t` can’t represent `((1U 

```
int32_t x = (1U 

#### Solution

Use a larger destination type, such as an `int64_t`.

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

Integer overflow

Detects overflow in arithmetic.

Invalid variable-length array

Detects negative array bounds.

