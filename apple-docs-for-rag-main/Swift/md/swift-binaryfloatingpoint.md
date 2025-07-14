

- Swift
-  BinaryFloatingPoint 

Protocol

# BinaryFloatingPoint

A radix-2 (binary) floating-point type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol BinaryFloatingPoint : ExpressibleByFloatLiteral, FloatingPoint
```

## Overview

The `BinaryFloatingPoint` protocol extends the `FloatingPoint` protocol with operations specific to floating-point binary types, as defined by the IEEE 754 specification. `BinaryFloatingPoint` is implemented in the standard library by `Float`, `Double`, and `Float80` where available.

## Topics

### Converting Floating-Point Values

init(Float)

Creates a new instance from the given value, rounded to the closest possible representation.

**Required** Default implementations provided.

init(Double)

Creates a new instance from the given value, rounded to the closest possible representation.

**Required** Default implementations provided.

init(Float80)

Creates a new instance from the given value, rounded to the closest possible representation.

**Required** Default implementations provided.

init&lt;Source>(Source)

Creates a new instance from the given value, rounded to the closest possible representation.

**Required** Default implementations provided.

### Converting with No Loss of Precision

init?&lt;Source>(exactly: Source)

Creates a new instance from the given value, if it can be represented exactly.

**Required** Default implementations provided.

### Creating a Random Value

static func random(in: ClosedRange&lt;Self>) -> Self

Returns a random value within the specified range.

static func random(in: Range&lt;Self>) -> Self

Returns a random value within the specified range.

static func random&lt;T>(in: ClosedRange&lt;Self>, using: inout T) -> Self

Returns a random value within the specified range, using the given generator as a source for randomness.

static func random&lt;T>(in: Range&lt;Self>, using: inout T) -> Self

Returns a random value within the specified range, using the given generator as a source for randomness.

### Working with Binary Representation

var binade: Self

The floating-point value with the same sign and exponent as this value, but with a significand of 1.0.

**Required**

var exponentBitPattern: Self.RawExponent

The raw encoding of the value’s exponent field.

**Required**

var significandBitPattern: Self.RawSignificand

The raw encoding of the value’s significand field.

**Required**

var significandWidth: Int

The number of bits required to represent the value’s significand.

**Required**

static var exponentBitCount: Int

The number of bits used to represent the type’s exponent.

**Required**

static var significandBitCount: Int

The available number of fractional significand bits.

**Required**

init(sign: FloatingPointSign, exponentBitPattern: Self.RawExponent, significandBitPattern: Self.RawSignificand)

Creates a new instance from the specified sign and bit patterns.

**Required**

associatedtype RawExponent : UnsignedInteger

A type that represents the encoded exponent of a value.

**Required**

associatedtype RawSignificand : UnsignedInteger

A type that represents the encoded significand of a value.

**Required**

### Initializers

init(String, format: FloatingPointFormatStyle&lt;Self>.Percent, lenient: Bool) throws

init(String, format: FloatingPointFormatStyle&lt;Self>.Currency, lenient: Bool) throws

init(String, format: FloatingPointFormatStyle&lt;Self>, lenient: Bool) throws

Initialize an instance by parsing `value` with a `ParseStrategy` created with the given `format` and the `lenient` argument.

init&lt;S>(S.ParseInput, strategy: S) throws

Initialize an instance by parsing `value` with the given `strategy`.

### Instance Methods

func formatted() -> String

Format `self` with `FloatingPointFormatStyle()`.

func formatted&lt;S>(S) -> S.FormatOutput

Format `self` with the given format.

func formatted&lt;S>(S) -> S.FormatOutput

Format `self` with the given format. `self` is first converted to `S.FormatInput` type, then format with the given format.

### Default Implementations

BinaryFloatingPoint Implementations

## Relationships

### Inherits From

- AdditiveArithmetic
- Comparable
- Equatable
- ExpressibleByFloatLiteral
- ExpressibleByIntegerLiteral
- FloatingPoint
- Hashable
- Numeric
- SignedNumeric
- Strideable

### Conforming Types

- Double
- Float
- Float16
- Float80

## See Also

### Floating Point

protocol FloatingPoint

A floating-point numeric type.

