

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Null reference creation and null pointer dereference 

Article

# Null reference creation and null pointer dereference

Detects the creation of null references and null pointer dereferences.

## Overview

In Xcode 9 and later, you can use this check to detect the creation of null references and null pointer dereferences. Dereferencing a null pointer always results in undefined behavior and can cause crashes. If the compiler finds a pointer dereference, it treats that pointer as nonnull. As a result, the optimizer may remove null equality checks for dereferenced pointers.

### Creating a null reference in C++

The following example demonstrates how to create a null reference. References in C++ must be nonnull:

```
int &x = *(int *)nullptr; // Error: null reference
```

#### Solution

Use a pointer instead.

```
int *x = nullptr; // Correct
```

### Member access through a null pointer in C++

The following code makes a member call on an object with a null address. The compiler may remove the null check on the `this` pointer because it requires the pointer to be `nonnull`.

```
struct A {
    int x;
    int getX() {
        if (!this) { // Warning: redundant null check may be removed
            return 0;
        }
        return x; // Warning: 'this' pointer is null, but is dereferenced here
    }
};
A *a = nullptr;
int x = a->getX(); // Error: member access through null pointer
```

Important

Always avoid null checks on the `this` pointer.

#### Solution

Avoid calling methods on null objects.

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

Invalid object size

Detects invalid pointer casts due to differences in the sizes of types.

Invalid shift

Detects invalid and overflowing shifts.

Integer overflow

Detects overflow in arithmetic.

Invalid variable-length array

Detects negative array bounds.

