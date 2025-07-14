

- Swift
-  Int16 

Structure

# Int16

A 16-bit signed integer value type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Int16
```

## Topics

### Structures

struct Words

A type that represents the words of this integer.

### Operators

static func != (Int16, Int16) -> Bool

static func &amp;= (inout Int16, Int16)

Stores the result of performing a bitwise AND operation on the two given values in the left-hand-side variable.

static func &amp;&lt;&lt;= (inout Int16, Int16)

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

static func &amp;>>= (inout Int16, Int16)

Calculates the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

static func *= (inout Int16, Int16)

Multiplies two values and stores the result in the left-hand-side variable.

static func += (inout Int16, Int16)

Adds two values and stores the result in the left-hand-side variable.

static func -= (inout Int16, Int16)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

static func == (Int16, Int16) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (Int16, Int16) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

static func /= (inout Int16, Int16)

Divides the first value by the second and stores the quotient in the left-hand-side variable.

static func %= (inout Int16, Int16)

Divides the first value by the second and stores the remainder in the left-hand-side variable.

static func ^= (inout Int16, Int16)

Stores the result of performing a bitwise XOR operation on the two given values in the left-hand-side variable.

static func |= (inout Int16, Int16)

Stores the result of performing a bitwise OR operation on the two given values in the left-hand-side variable.

### Initializers

init(Float16)

Creates an integer from the given floating-point value, rounding toward zero.

init(Float)

Creates an integer from the given floating-point value, rounding toward zero.

init(CGFloat)

init(Double)

Creates an integer from the given floating-point value, rounding toward zero.

init(Float80)

Creates an integer from the given floating-point value, rounding toward zero.

init(NSNumber)

init(bitPattern: UInt16)

Creates a new instance with the same memory representation as the given value.

init?(exactly: Float80)

Creates an integer from the given floating-point value, if it can be represented exactly.

init?(exactly: Double)

Creates an integer from the given floating-point value, if it can be represented exactly.

init?(exactly: Float16)

Creates an integer from the given floating-point value, if it can be represented exactly.

init?(exactly: NSNumber)

init?(exactly: Float)

Creates an integer from the given floating-point value, if it can be represented exactly.

init(truncating: NSNumber)

### Instance Properties

var byteSwapped: Int16

A representation of this integer with the byte order swapped.

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `Int16` instance.

Deprecated

var leadingZeroBitCount: Int

The number of leading zeros in this value’s binary representation.

var magnitude: UInt16

The magnitude of this value.

var nonzeroBitCount: Int

The number of bits equal to 1 in this value’s binary representation.

var trailingZeroBitCount: Int

The number of trailing zeros in this value’s binary representation.

var words: Int16.Words

A collection containing the words of this value’s binary representation, in order from the least significant to most significant.

### Instance Methods

func addingReportingOverflow(Int16) -> (partialValue: Int16, overflow: Bool)

Returns the sum of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func dividedReportingOverflow(by: Int16) -> (partialValue: Int16, overflow: Bool)

Returns the quotient obtained by dividing this value by the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func dividingFullWidth((high: Int16, low: Int16.Magnitude)) -> (quotient: Int16, remainder: Int16)

Returns a tuple containing the quotient and remainder of dividing the given value by this value.

func multipliedFullWidth(by: Int16) -> (high: Int16, low: Int16.Magnitude)

Returns a tuple containing the high and low parts of the result of multiplying this value by the given value.

func multipliedReportingOverflow(by: Int16) -> (partialValue: Int16, overflow: Bool)

Returns the product of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func remainderReportingOverflow(dividingBy: Int16) -> (partialValue: Int16, overflow: Bool)

Returns the remainder after dividing this value by the given value, along with a Boolean value indicating whether overflow occurred during division.

func signum() -> Int16

Returns `-1` if this value is negative and `1` if it’s positive; otherwise, `0`.

func subtractingReportingOverflow(Int16) -> (partialValue: Int16, overflow: Bool)

Returns the difference obtained by subtracting the given value from this value, along with a Boolean value indicating whether overflow occurred in the operation.

### Type Aliases

typealias IntegerLiteralType

A type that represents an integer literal.

typealias Magnitude

A type that can represent the absolute value of any possible value of this type.

typealias Stride

A type that represents the distance between two values.

### Type Properties

static var bitWidth: Int

The number of bits used for the underlying binary representation of values of this type.

### Default Implementations

AdditiveArithmetic Implementations

AtomicRepresentable Implementations

BinaryInteger Implementations

Comparable Implementations

CustomReflectable Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

ExpressibleByIntegerLiteral Implementations

FixedWidthInteger Implementations

Hashable Implementations

SIMDScalar Implementations

SignedInteger Implementations

SignedNumeric Implementations

## Relationships

### Conforms To

- AdditiveArithmetic
- AtomicRepresentable
- BNNSScalar
- BinaryInteger
- BitwiseCopyable
- CKRecordValueProtocol
- CVarArg
- Comparable
- Copyable
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByIntegerLiteral
- FixedWidthInteger
- Hashable
- LosslessStringConvertible
- MLTensorScalar
- Numeric
- Plottable
- PrimitivePlottableProtocol
- SIMDScalar
- Sendable
- SignedInteger
- SignedNumeric
- Strideable
- vDSP_IntegerConvertable

## See Also

### Signed Integers

struct Int8

An 8-bit signed integer value type.

struct Int32

A 32-bit signed integer value type.

struct Int64

A 64-bit signed integer value type.

struct Int128

A 128-bit signed integer value type.

