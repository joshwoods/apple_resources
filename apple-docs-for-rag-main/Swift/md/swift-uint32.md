

- Swift
-  UInt32 

Structure

# UInt32

A 32-bit unsigned integer value type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct UInt32
```

## Topics

### Structures

struct Words

A type that represents the words of this integer.

### Operators

static func != (UInt32, UInt32) -> Bool

static func &amp;= (inout UInt32, UInt32)

Stores the result of performing a bitwise AND operation on the two given values in the left-hand-side variable.

static func &amp;&lt;&lt;= (inout UInt32, UInt32)

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

static func &amp;>>= (inout UInt32, UInt32)

Calculates the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

static func *= (inout UInt32, UInt32)

Multiplies two values and stores the result in the left-hand-side variable.

static func += (inout UInt32, UInt32)

Adds two values and stores the result in the left-hand-side variable.

static func -= (inout UInt32, UInt32)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

static func == (UInt32, UInt32) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (UInt32, UInt32) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

static func |= (inout UInt32, UInt32)

Stores the result of performing a bitwise OR operation on the two given values in the left-hand-side variable.

static func %= (inout UInt32, UInt32)

Divides the first value by the second and stores the remainder in the left-hand-side variable.

static func /= (inout UInt32, UInt32)

Divides the first value by the second and stores the quotient in the left-hand-side variable.

static func ^= (inout UInt32, UInt32)

Stores the result of performing a bitwise XOR operation on the two given values in the left-hand-side variable.

### Initializers

init(Float)

Creates an integer from the given floating-point value, rounding toward zero.

init(Float16)

Creates an integer from the given floating-point value, rounding toward zero.

init(Float80)

Creates an integer from the given floating-point value, rounding toward zero.

init(Unicode.Scalar)

Construct with value `v.value`.

init(CGFloat)

init(NSNumber)

init(Double)

Creates an integer from the given floating-point value, rounding toward zero.

init(bitPattern: Int32)

Creates a new instance with the same memory representation as the given value.

init?(exactly: NSNumber)

init?(exactly: Float80)

Creates an integer from the given floating-point value, if it can be represented exactly.

init?(exactly: Double)

Creates an integer from the given floating-point value, if it can be represented exactly.

init?(exactly: Float16)

Creates an integer from the given floating-point value, if it can be represented exactly.

init?(exactly: Float)

Creates an integer from the given floating-point value, if it can be represented exactly.

init(truncating: NSNumber)

### Instance Properties

var byteSwapped: UInt32

A representation of this integer with the byte order swapped.

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `UInt32` instance.

Deprecated

var leadingZeroBitCount: Int

The number of leading zeros in this value’s binary representation.

var nonzeroBitCount: Int

The number of bits equal to 1 in this value’s binary representation.

var trailingZeroBitCount: Int

The number of trailing zeros in this value’s binary representation.

var words: UInt32.Words

A collection containing the words of this value’s binary representation, in order from the least significant to most significant.

### Instance Methods

func addingReportingOverflow(UInt32) -> (partialValue: UInt32, overflow: Bool)

Returns the sum of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func dividedReportingOverflow(by: UInt32) -> (partialValue: UInt32, overflow: Bool)

Returns the quotient obtained by dividing this value by the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func dividingFullWidth((high: UInt32, low: UInt32.Magnitude)) -> (quotient: UInt32, remainder: UInt32)

Returns a tuple containing the quotient and remainder of dividing the given value by this value.

func multipliedFullWidth(by: UInt32) -> (high: UInt32, low: UInt32.Magnitude)

Returns a tuple containing the high and low parts of the result of multiplying this value by the given value.

func multipliedReportingOverflow(by: UInt32) -> (partialValue: UInt32, overflow: Bool)

Returns the product of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func remainderReportingOverflow(dividingBy: UInt32) -> (partialValue: UInt32, overflow: Bool)

Returns the remainder after dividing this value by the given value, along with a Boolean value indicating whether overflow occurred during division.

func signum() -> UInt32

Returns `-1` if this value is negative and `1` if it’s positive; otherwise, `0`.

func subtractingReportingOverflow(UInt32) -> (partialValue: UInt32, overflow: Bool)

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

UnsignedInteger Implementations

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
- Strideable
- UnsignedInteger
- vDSP_IntegerConvertable

## See Also

### Unsigned Integers

struct UInt

An unsigned integer value type.

struct UInt8

An 8-bit unsigned integer value type.

struct UInt16

A 16-bit unsigned integer value type.

struct UInt64

A 64-bit unsigned integer value type.

struct UInt128

A 128-bit unsigned integer value type.

