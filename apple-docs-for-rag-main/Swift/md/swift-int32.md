

- Swift
-  Int32 

Structure

# Int32

A 32-bit signed integer value type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Int32
```

## Topics

### Structures

struct Words

A type that represents the words of this integer.

### Operators

static func != (Int32, Int32) -> Bool

static func &amp;= (inout Int32, Int32)

Stores the result of performing a bitwise AND operation on the two given values in the left-hand-side variable.

static func &amp;&lt;&lt;= (inout Int32, Int32)

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

static func &amp;>>= (inout Int32, Int32)

Calculates the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

static func *= (inout Int32, Int32)

Multiplies two values and stores the result in the left-hand-side variable.

static func += (inout Int32, Int32)

Adds two values and stores the result in the left-hand-side variable.

static func -= (inout Int32, Int32)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

static func == (Int32, Int32) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (Int32, Int32) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

static func ^= (inout Int32, Int32)

Stores the result of performing a bitwise XOR operation on the two given values in the left-hand-side variable.

static func |= (inout Int32, Int32)

Stores the result of performing a bitwise OR operation on the two given values in the left-hand-side variable.

static func %= (inout Int32, Int32)

Divides the first value by the second and stores the remainder in the left-hand-side variable.

static func /= (inout Int32, Int32)

Divides the first value by the second and stores the quotient in the left-hand-side variable.

### Initializers

init(Float80)

Creates an integer from the given floating-point value, rounding toward zero.

init(Float)

Creates an integer from the given floating-point value, rounding toward zero.

init(Float16)

Creates an integer from the given floating-point value, rounding toward zero.

init(NSNumber)

init(CGFloat)

init(Double)

Creates an integer from the given floating-point value, rounding toward zero.

init(bitPattern: UInt32)

Creates a new instance with the same memory representation as the given value.

init?(exactly: Float16)

Creates an integer from the given floating-point value, if it can be represented exactly.

init?(exactly: NSNumber)

init?(exactly: Double)

Creates an integer from the given floating-point value, if it can be represented exactly.

init?(exactly: Float80)

Creates an integer from the given floating-point value, if it can be represented exactly.

init?(exactly: Float)

Creates an integer from the given floating-point value, if it can be represented exactly.

init(truncating: NSNumber)

### Instance Properties

var byteSwapped: Int32

A representation of this integer with the byte order swapped.

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `Int32` instance.

Deprecated

var leadingZeroBitCount: Int

The number of leading zeros in this value’s binary representation.

var magnitude: UInt32

The magnitude of this value.

var nonzeroBitCount: Int

The number of bits equal to 1 in this value’s binary representation.

var trailingZeroBitCount: Int

The number of trailing zeros in this value’s binary representation.

var words: Int32.Words

A collection containing the words of this value’s binary representation, in order from the least significant to most significant.

### Instance Methods

func addingReportingOverflow(Int32) -> (partialValue: Int32, overflow: Bool)

Returns the sum of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func dividedReportingOverflow(by: Int32) -> (partialValue: Int32, overflow: Bool)

Returns the quotient obtained by dividing this value by the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func dividingFullWidth((high: Int32, low: Int32.Magnitude)) -> (quotient: Int32, remainder: Int32)

Returns a tuple containing the quotient and remainder of dividing the given value by this value.

func multipliedFullWidth(by: Int32) -> (high: Int32, low: Int32.Magnitude)

Returns a tuple containing the high and low parts of the result of multiplying this value by the given value.

func multipliedReportingOverflow(by: Int32) -> (partialValue: Int32, overflow: Bool)

Returns the product of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func remainderReportingOverflow(dividingBy: Int32) -> (partialValue: Int32, overflow: Bool)

Returns the remainder after dividing this value by the given value, along with a Boolean value indicating whether overflow occurred during division.

func signum() -> Int32

Returns `-1` if this value is negative and `1` if it’s positive; otherwise, `0`.

func subtractingReportingOverflow(Int32) -> (partialValue: Int32, overflow: Bool)

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

static var mlMultiArrayDataType: MLMultiArrayDataType

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
- MLShapedArrayScalar
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

struct Int16

A 16-bit signed integer value type.

struct Int64

A 64-bit signed integer value type.

struct Int128

A 128-bit signed integer value type.

