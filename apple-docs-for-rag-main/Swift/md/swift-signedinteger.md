

- Swift
-  SignedInteger 

Protocol

# SignedInteger

An integer type that can represent both positive and negative values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol SignedInteger : BinaryInteger, SignedNumeric
```

## Topics

### Instance Methods

func dividingFullWidth((high: Self, low: Self.Magnitude)) -> (quotient: Self, remainder: Self)

### Type Properties

static var max: Self

The maximum representable integer in this type.

static var min: Self

The minimum representable integer in this type.

## Relationships

### Inherits From

- AdditiveArithmetic
- BinaryInteger
- Comparable
- CustomStringConvertible
- Equatable
- ExpressibleByIntegerLiteral
- Hashable
- Numeric
- SignedNumeric
- Strideable

### Conforming Types

- Int
- Int128
- Int16
- Int32
- Int64
- Int8

## See Also

### Integer

protocol BinaryInteger

An integer type with a binary representation.

protocol FixedWidthInteger

An integer type that uses a fixed size for every instance.

protocol UnsignedInteger

An integer type that can represent only nonnegative values.

