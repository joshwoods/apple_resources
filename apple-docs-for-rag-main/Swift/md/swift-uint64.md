

- Swift
-  UInt64 

Structure

# UInt64

A 64-bit unsigned integer value type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct UInt64
```

## Topics

### Structures

struct Words

A type that represents the words of this integer.

### Operators

static func != (UInt64, UInt64) -> Bool

static func &amp;= (inout UInt64, UInt64)

Stores the result of performing a bitwise AND operation on the two given values in the left-hand-side variable.

static func &amp;>>= (inout UInt64, UInt64)

Calculates the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

static func &amp;&lt;&lt;= (inout UInt64, UInt64)

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

static func *= (inout UInt64, UInt64)

Multiplies two values and stores the result in the left-hand-side variable.

static func += (inout UInt64, UInt64)

Adds two values and stores the result in the left-hand-side variable.

static func -= (inout UInt64, UInt64)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

static func == (UInt64, UInt64) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (UInt64, UInt64) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

static func %= (inout UInt64, UInt64)

Divides the first value by the second and stores the remainder in the left-hand-side variable.

static func |= (inout UInt64, UInt64)

Stores the result of performing a bitwise OR operation on the two given values in the left-hand-side variable.

static func ^= (inout UInt64, UInt64)

Stores the result of performing a bitwise XOR operation on the two given values in the left-hand-side variable.

static func /= (inout UInt64, UInt64)

Divides the first value by the second and stores the quotient in the left-hand-side variable.

### Initializers

init(CGFloat)

init(Float16)

Creates an integer from the given floating-point value, rounding toward zero.

init(Double)

Creates an integer from the given floating-point value, rounding toward zero.

init(NSNumber)

init(Unicode.Scalar)

Construct with value `v.value`.

init(Float80)

Creates an integer from the given floating-point value, rounding toward zero.

init(Float)

Creates an integer from the given floating-point value, rounding toward zero.

init(bitPattern: Int64)

Creates a new instance with the same memory representation as the given value.

init?(exactly: Float80)

Creates an integer from the given floating-point value, if it can be represented exactly.

init?(exactly: NSNumber)

init?(exactly: Double)

Creates an integer from the given floating-point value, if it can be represented exactly.

init?(exactly: Float16)

Creates an integer from the given floating-point value, if it can be represented exactly.

init?(exactly: Float)

Creates an integer from the given floating-point value, if it can be represented exactly.

init(truncating: NSNumber)

### Instance Properties

var byteSwapped: UInt64

A representation of this integer with the byte order swapped.

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `UInt64` instance.

Deprecated

var leadingZeroBitCount: Int

The number of leading zeros in this value’s binary representation.

var nonzeroBitCount: Int

The number of bits equal to 1 in this value’s binary representation.

var trailingZeroBitCount: Int

The number of trailing zeros in this value’s binary representation.

var words: UInt64.Words

A collection containing the words of this value’s binary representation, in order from the least significant to most significant.

### Instance Methods

func addingReportingOverflow(UInt64) -> (partialValue: UInt64, overflow: Bool)

Returns the sum of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func dividedReportingOverflow(by: UInt64) -> (partialValue: UInt64, overflow: Bool)

Returns the quotient obtained by dividing this value by the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func dividingFullWidth((high: UInt64, low: UInt64.Magnitude)) -> (quotient: UInt64, remainder: UInt64)

Returns a tuple containing the quotient and remainder of dividing the given value by this value.

func multipliedFullWidth(by: UInt64) -> (high: UInt64, low: UInt64.Magnitude)

Returns a tuple containing the high and low parts of the result of multiplying this value by the given value.

func multipliedReportingOverflow(by: UInt64) -> (partialValue: UInt64, overflow: Bool)

Returns the product of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func remainderReportingOverflow(dividingBy: UInt64) -> (partialValue: UInt64, overflow: Bool)

Returns the remainder after dividing this value by the given value, along with a Boolean value indicating whether overflow occurred during division.

func signum() -> UInt64

Returns `-1` if this value is negative and `1` if it’s positive; otherwise, `0`.

func subtractingReportingOverflow(UInt64) -> (partialValue: UInt64, overflow: Bool)

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
- Numeric
- Plottable
- PrimitivePlottableProtocol
- SIMDScalar
- Sendable
- Strideable
- SynchronizationPeerID
- UnsignedInteger

## See Also

### Unsigned Integers

struct UInt

An unsigned integer value type.

struct UInt8

An 8-bit unsigned integer value type.

struct UInt16

A 16-bit unsigned integer value type.

struct UInt32

A 32-bit unsigned integer value type.

struct UInt128

A 128-bit unsigned integer value type.

