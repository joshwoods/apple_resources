

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Misaligned pointer 

Article

# Misaligned pointer

Detects when code accesses a misaligned pointer or creates a misaligned reference.

## Overview

In Xcode 9 and later, you can use this check to detect reads from, or writes to, a misaligned pointer, or when you create a misaligned reference. A pointer misaligns if its address isn’t a multiple of its type’s alignment. Dereferencing a misaligned pointer has undefined behavior, and may result in a crash or degraded performance.

Alignment violations occur frequently in code that serializes or deserializes data. Avoid this issue by using a serialization format that preserves data alignment.

### Misaligned integer pointer assignment in C

In the following example, the `pointer` variable must have 4-byte alignment, but has only 1-byte alignment:

```
int8_t *buffer = malloc(64);
int32_t *pointer = (int32_t *)(buffer + 1);
*pointer = 42; // Error: misaligned integer pointer assignment
```

#### Solution

Use an assignment function like `memcpy`, which can work with unaligned inputs.

```
int8_t *buffer = malloc(64);
int32_t value = 42;
memcpy(buffer + 1, &value, sizeof(int32_t)); // Correct
```

Note

The compiler can often safely optimize calls to `memcpy`, even for unaligned arguments.

### Misaligned structure pointer assignment in C

In the following example, the `pointer` variable must have 8-byte alignment, but has only 1-byte alignment:

```
struct A {
    int32_t i32;
    int64_t i64;
};
int8_t *buffer = malloc(32);
struct A *pointer = (struct A *)(buffer + 1);
pointer->i32 = 7; // Error: pointer is misaligned
```

#### Solution

One solution is to pack the structure. In the following example, the packed `A` structure prevents the compiler from adding padding between members:

```
struct A { ... } __attribute__((packed));
```

Important

Packing a structure may adversely impact performance.

## See Also

### Undefined Behavior Sanitizer

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

Integer overflow

Detects overflow in arithmetic.

Invalid variable-length array

Detects negative array bounds.

