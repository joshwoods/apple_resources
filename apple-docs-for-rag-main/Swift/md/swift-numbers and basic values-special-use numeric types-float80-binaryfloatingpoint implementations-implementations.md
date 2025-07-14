

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Numbers and Basic Values
- Special-Use Numeric Types
- Float80
-  BinaryFloatingPoint Implementations 

API Collection

# BinaryFloatingPoint Implementations

## Topics

### Initializers

init(Double)

Creates a new instance that approximates the given value.

init(Float)

Creates a new instance that approximates the given value.

init&lt;Source>(Source)

Creates a new instance from the given value, rounded to the closest possible representation.

init(Float80)

Creates a new instance initialized to the given value.

init&lt;Source>(Source)

Creates a new value, rounded to the closest possible representation.

init?&lt;Source>(exactly: Source)

Creates a new value, if the given integer can be represented exactly.

init?&lt;Source>(exactly: Source)

Creates a new instance from the given value, if it can be represented exactly.

init(sign: FloatingPointSign, exponentBitPattern: UInt, significandBitPattern: UInt64)

Creates a new instance from the specified sign and bit patterns.

### Instance Properties

var binade: Float80

The floating-point value with the same sign and exponent as this value, but with a significand of 1.0.

var exponentBitPattern: UInt

The raw encoding of the value’s exponent field.

var significandBitPattern: UInt64

The raw encoding of the value’s significand field.

var significandWidth: Int

The number of bits required to represent the value’s significand.

### Type Aliases

typealias RawExponent

A type that represents the encoded exponent of a value.

typealias RawSignificand

A type that represents the encoded significand of a value.

### Type Properties

static var exponentBitCount: Int

The number of bits used to represent the type’s exponent.

static var significandBitCount: Int

The available number of fractional significand bits.

### Type Methods

static func random(in: Range&lt;Self>) -> Self

Returns a random value within the specified range.

static func random(in: ClosedRange&lt;Self>) -> Self

Returns a random value within the specified range.

static func random&lt;T>(in: ClosedRange&lt;Self>, using: inout T) -> Self

Returns a random value within the specified range, using the given generator as a source for randomness.

static func random&lt;T>(in: Range&lt;Self>, using: inout T) -> Self

Returns a random value within the specified range, using the given generator as a source for randomness.

