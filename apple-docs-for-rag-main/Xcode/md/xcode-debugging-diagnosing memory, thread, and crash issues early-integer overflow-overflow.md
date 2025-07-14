

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Integer overflow 

Article

# Integer overflow

Detects overflow in arithmetic.

## Overview

Overflows result in undefined behavior. Use this check to detect overflows in addition, subtraction, multiplication, and division. Available in Xcode 9 and later.

### Signed addition overflow in C

In the following code, the `x` variable has the maximum `int32_t` value before the addition, and the result of the addition overflows `x`, which the optimizer may not handle in a predictable way:

```
int32_t x = (1U 

Note

With the exception of the signed division check, enabling the `-fwrapv` compiler flag disables UBSan overflow checks.

#### Solution

One way to address signed overflow is to use larger types.

If you don’t need to represent negative numbers, another option is to use unsigned types, which wrap on arithmetic overflow. Alternatively, pass the `-fwrapv` flag to the compiler to enable signed wraparound on overflow. However, this may adversely impact performance.

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

Invalid variable-length array

Detects negative array bounds.

