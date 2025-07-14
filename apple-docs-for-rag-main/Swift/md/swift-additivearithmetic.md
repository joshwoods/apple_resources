

- Swift
-  AdditiveArithmetic 

Protocol

# AdditiveArithmetic

A type with values that support addition and subtraction.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol AdditiveArithmetic : Equatable
```

## Overview

The `AdditiveArithmetic` protocol provides a suitable basis for additive arithmetic on scalar values, such as integers and floating-point numbers, or vectors. You can write generic methods that operate on any numeric type in the standard library by using the `AdditiveArithmetic` protocol as a generic constraint.

The following code declares a method that calculates the total of any sequence with `AdditiveArithmetic` elements.

```
extension Sequence where Element: AdditiveArithmetic {
    func sum() -> Element {
        return reduce(.zero, +)
    }
}
```

The `sum()` method is now available on any sequence with values that conform to `AdditiveArithmetic`, whether it is an array of `Double` or a range of `Int`.

```
let arraySum = [1.1, 2.2, 3.3, 4.4, 5.5].sum()
// arraySum == 16.5

let rangeSum = (1..

# Conforming to the AdditiveArithmetic Protocol

To add `AdditiveArithmetic` protocol conformance to your own custom type, implement the required operators, and provide a static `zero` property.

## Topics

### Operators

static func + (Self) -> Self

Returns the given number unchanged.

static func + (Self, Self) -> Self

Adds two values and produces their sum.

**Required**

static func += (inout Self, Self)

Adds two values and stores the result in the left-hand-side variable.

**Required** Default implementation provided.

static func - (Self, Self) -> Self

Subtracts one value from another and produces their difference.

**Required**

static func -= (inout Self, Self)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

**Required** Default implementation provided.

### Type Properties

static var zero: Self

The zero value.

**Required** Default implementation provided.

## Relationships

### Inherits From

- Equatable

### Inherited By

- BinaryFloatingPoint
- BinaryInteger
- DurationProtocol
- FixedWidthInteger
- FloatingPoint
- Numeric
- SignedInteger
- SignedNumeric
- UnsignedInteger

### Conforming Types

- Double
- Duration
- Float
- Float16
- Float80
- Int
- Int128
- Int16
- Int32
- Int64
- Int8
- UInt
- UInt128
- UInt16
- UInt32
- UInt64
- UInt8

## See Also

### Basic Arithmetic

protocol Numeric

A type with values that support multiplication.

protocol SignedNumeric

A numeric type with a negation operation.

protocol Strideable

A type representing continuous, one-dimensional values that can be offset and measured.

