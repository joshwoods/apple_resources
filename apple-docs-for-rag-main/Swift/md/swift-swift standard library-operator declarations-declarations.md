

- Swift
- Swift Standard Library
-  Operator Declarations 

Article

# Operator Declarations

Work with prefix, postfix, and infix operators.

## Overview

The tables below list the operators declared by the Swift standard library. For more information about operation declarations, see Operator Declaration in The Swift Programming Language.

The prefix operators are as follows:

| Operator | Description           |
|----------|-----------------------|
| `!`      | Logical NOT           |
| `.!`     | Pointwise logical NOT |
| `~`      | Bitwise NOT           |
| `+`      | Unary plus            |
| `-`      | Unary minus           |
| `..

The postfix operators are as follows:

| Operator | Description |
|----------|-------------|
| `...`    | Range       |

The infix operators are grouped below by precedence group in decreasing order of precedence. If you declare a new operator without specifying a precedence group, it is a member of the `DefaultPrecedence` precedence group. `DefaultPrecedence` has no associativity and a precedence immediately higher than `TernaryPrecedence`.

The `BitwiseShiftPrecedence` group, which isn’t associative, contains the following infix operators:

| Operator | Description                            |
|----------|----------------------------------------|
| `>`     | Bitwise right shift                    |
| `&>`    | Bitwise right shift, ignoring overflow |

The `MultiplicationPrecedence` group, which is left associative, contains the following infix operators:

| Operator | Description            |
|----------|------------------------|
| `*`      | Multiply               |
| `/`      | Divide                 |
| `%`      | Remainder              |
| `&`      | Bitwise AND            |
| `&*`     | Multiply with overflow |

The `AdditionPrecedence` group, which is left associative, contains the following infix operators:

| Operator | Description            |
|----------|------------------------|
| `+`      | Add                    |
| `-`      | Subtract               |
| `|`      | Bitwise OR             |
| `^`      | Bitwise XOR            |
| `&+`     | Add with overflow      |
| `&-`     | Subtract with overflow |

The `RangeFormationPrecedence` group, which isn’t associative, contains the following infix operators:

| Operator | Description     |
|----------|-----------------|
| `..

The `CastingPrecedence` group, which is left associative, contains the following infix operators:

| Operator               | Description |
|------------------------|-------------|
| `is`                   | Type check  |
| `as`, `as?`, and `as!` | Type cast   |

The `NilCoalescingPrecedence` group, which is right associative, contains the following infix operators:

| Operator | Description    |
|----------|----------------|
| `??`     | Nil coalescing |

The `ComparisonPrecedence` group, which isn’t associative, contains the following infix operators:

| Operator | Description                     |
|----------|---------------------------------|
| ``      | Greater than                    |
| `>=`     | Greater than or equal           |
| `==`     | Equal                           |
| `!=`     | Not equal                       |
| `===`    | Identical                       |
| `!==`    | Not identical                   |
| `~=`     | Pattern match                   |
| `.`     | Pointwise greater than          |
| `.>=`    | Pointwise greater than or equal |
| `.==`    | Pointwise equal                 |
| `.!=`    | Pointwise not equal             |

The `LogicalConjunctionPrecedence` group, which is left associative, contains the following infix operators:

| Operator | Description           |
|----------|-----------------------|
| `&&`     | Logical AND           |
| `.&`     | Pointwise bitwise AND |

The `LogicalDisjunctionPrecedence` group, which is left associative, contains the following infix operators:

| Operator | Description           |
|----------|-----------------------|
| `||`     | Logical OR            |
| `.|`     | Pointwise bitwise OR  |
| `.^`     | Pointwise bitwise XOR |

The `TernaryPrecedence` group, which is right associative, contains the following infix operators:

| Operator | Description         |
|----------|---------------------|
| `?` `:`  | Ternary conditional |

The `AssignmentPrecedence` group, which is right associative, contain the following infix operators:

| Operator | Description                                  |
|----------|----------------------------------------------|
| `=`      | Assign                                       |
| `*=`     | Multiply and assign                          |
| `/=`     | Divide and assign                            |
| `%=`     | Remainder and assign                         |
| `+=`     | Add and assign                               |
| `-=`     | Subtract and assign                          |
| `>=`    | Right bit shift and assign                   |
| `&=`     | Bitwise AND and assign                       |
| `|=`     | Bitwise OR and assign                        |
| `^=`     | Bitwise XOR and assign                       |
| `&*=`    | Multiply with overflow and assign            |
| `&+=`    | Add with overflow and assign                 |
| `&-=`    | Subtract with overflow and assign            |
| `&>=`   | Right bit shift ignoring overflow and assign |
| `.&=`    | Pointwise bitwise AND and assign             |
| `.|=`    | Pointwise bitwise OR and assign              |
| `.^=`    | Pointwise bitwise XOR and assign             |

## See Also

### Programming Tasks

Input and Output

Print values to the console, read from and write to text streams, and use command line arguments.

Debugging and Reflection

Fortify your code with runtime checks, and examine your values’ runtime representation.

Macros

Generate boilerplate code and perform other compile-time operations.

Concurrency

Perform asynchronous and parallel operations.

Key-Path Expressions

Use key-path expressions to access properties dynamically.

Manual Memory Management

Allocate and manage memory manually.

Type Casting and Existential Types

Perform casts between types or represent values of any type.

C Interoperability

Use imported C types or call C variadic functions.

