

- Swift
-  SignedNumeric 

Protocol

# SignedNumeric

A numeric type with a negation operation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol SignedNumeric : Numeric
```

## Overview

The `SignedNumeric` protocol extends the operations defined by the `Numeric` protocol to include a value’s additive inverse.

# Conforming to the SignedNumeric Protocol

Because the `SignedNumeric` protocol provides default implementations of both of its required methods, you don’t need to do anything beyond declaring conformance to the protocol and ensuring that the values of your type support negation. To customize your type’s implementation, provide your own mutating `negate()` method.

When the additive inverse of a value is unrepresentable in a conforming type, the operation should either trap or return an exceptional value. For example, using the negation operator (prefix `-`) with `Int.min` results in a runtime error.

```
let x = Int.min
let y = -x
// Overflow error
```

## Topics

### Operators

static func - (Self) -> Self

Returns the additive inverse of the specified value.

**Required** Default implementation provided.

### Instance Methods

func negate()

Replaces this value with its additive inverse.

**Required** Default implementation provided.

## Relationships

### Inherits From

- AdditiveArithmetic
- Equatable
- ExpressibleByIntegerLiteral
- Numeric

### Inherited By

- BinaryFloatingPoint
- FloatingPoint
- SignedInteger

### Conforming Types

- Double
- Float
- Float16
- Float80
- Int
- Int128
- Int16
- Int32
- Int64
- Int8

## See Also

### Basic Arithmetic

protocol AdditiveArithmetic

A type with values that support addition and subtraction.

protocol Numeric

A type with values that support multiplication.

protocol Strideable

A type representing continuous, one-dimensional values that can be offset and measured.

