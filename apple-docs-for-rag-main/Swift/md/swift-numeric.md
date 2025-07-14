

- Swift
-  Numeric 

Protocol

# Numeric

A type with values that support multiplication.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol Numeric : AdditiveArithmetic, ExpressibleByIntegerLiteral
```

## Overview

The `Numeric` protocol provides a suitable basis for arithmetic on scalar values, such as integers and floating-point numbers. You can write generic methods that operate on any numeric type in the standard library by using the `Numeric` protocol as a generic constraint.

The following example extends `Sequence` with a method that returns an array with the sequence’s values multiplied by two.

```
extension Sequence where Element: Numeric {
    func doublingAll() -> [Element] {
        return map { $0 * 2 }
    }
}
```

With this extension, any sequence with elements that conform to `Numeric` has the `doublingAll()` method. For example, you can double the elements of an array of doubles or a range of integers:

```
let observations = [1.5, 2.0, 3.25, 4.875, 5.5]
let doubledObservations = observations.doublingAll()
// doubledObservations == [3.0, 4.0, 6.5, 9.75, 11.0]

let integers = 0..

# Conforming to the Numeric Protocol

To add `Numeric` protocol conformance to your own custom type, implement the required initializer and operators, and provide a `magnitude` property using a type that can represent the magnitude of any value of your custom type.

## Topics

### Operators

static func * (Self, Self) -> Self

Multiplies two values and produces their product.

**Required**

static func *= (inout Self, Self)

Multiplies two values and stores the result in the left-hand-side variable.

**Required**

### Associated Types

associatedtype Magnitude : Comparable, Numeric

A type that can represent the absolute value of any possible value of the conforming type.

**Required**

### Initializers

init?&lt;T>(exactly: T)

Creates a new instance from the given integer, if it can be represented exactly.

**Required** Default implementations provided.

### Instance Properties

var magnitude: Self.Magnitude

The magnitude of this value.

**Required** Default implementation provided.

## Relationships

### Inherits From

- AdditiveArithmetic
- Equatable
- ExpressibleByIntegerLiteral

### Inherited By

- BinaryFloatingPoint
- BinaryInteger
- FixedWidthInteger
- FloatingPoint
- SignedInteger
- SignedNumeric
- UnsignedInteger

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
- UInt
- UInt128
- UInt16
- UInt32
- UInt64
- UInt8

## See Also

### Basic Arithmetic

protocol AdditiveArithmetic

A type with values that support addition and subtraction.

protocol SignedNumeric

A numeric type with a negation operation.

protocol Strideable

A type representing continuous, one-dimensional values that can be offset and measured.

