

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Numbers and Basic Values
- Special-Use Numeric Types
- Int128
-  FixedWidthInteger Implementations 

API Collection

# FixedWidthInteger Implementations

## Topics

### Operators

static func &amp;* (Int128, Int128) -> Int128

Returns the product of the two given values, wrapping the result in case of any overflow.

static func &amp;* (Self, Self) -> Self

Returns the product of the two given values, wrapping the result in case of any overflow.

static func &amp;*= (inout Self, Self)

Multiplies two values and stores the result in the left-hand-side variable, wrapping any overflow.

static func &amp;+ (Self, Self) -> Self

Returns the sum of the two given values, wrapping the result in case of any overflow.

static func &amp;+= (inout Self, Self)

Adds two values and stores the result in the left-hand-side variable, wrapping any overflow.

static func &amp;- (Self, Self) -> Self

Returns the difference of the two given values, wrapping the result in case of any overflow.

static func &amp;-= (inout Self, Self)

Subtracts the second value from the first and stores the difference in the left-hand-side variable, wrapping any overflow.

static func &amp;>> &lt;Other>(Self, Other) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width.

static func &amp;>> (Self, Self) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width.

static func &amp;&lt;&lt; &lt;Other>(Self, Other) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width.

static func &amp;&lt;&lt; (Self, Self) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width.

static func &amp;&lt;&lt;= &lt;Other>(inout Self, Other)

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

static func &amp;&lt;&lt;= (inout Int128, Int128)

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

static func &amp;>>= &lt;Other>(inout Self, Other)

Calculates the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

static func &amp;>>= (inout Int128, Int128)

Calculates the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

### Initializers

init&lt;T>(T)

init?(String)

Creates a new integer value from the given string.

init?&lt;S>(S, radix: Int)

Creates a new integer value from the given string and radix.

init(bigEndian: Self)

Creates an integer from its big-endian representation, changing the byte order if necessary.

init?&lt;T>(exactly: T)

init(littleEndian: Self)

Creates an integer from its little-endian representation, changing the byte order if necessary.

### Instance Properties

var bigEndian: Self

The big-endian representation of this integer.

var byteSwapped: Int128

A representation of this integer with the byte order swapped.

var leadingZeroBitCount: Int

The number of leading zeros in this value’s binary representation.

var littleEndian: Self

The little-endian representation of this integer.

var nonzeroBitCount: Int

The number of bits equal to 1 in this value’s binary representation.

### Instance Methods

func addingReportingOverflow(Int128) -> (partialValue: Int128, overflow: Bool)

Returns the sum of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func dividedReportingOverflow(by: Int128) -> (partialValue: Int128, overflow: Bool)

Returns the quotient obtained by dividing this value by the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func multipliedFullWidth(by: Self) -> (high: Self, low: Self.Magnitude)

Returns a tuple containing the high and low parts of the result of multiplying this value by the given value.

func multipliedReportingOverflow(by: Int128) -> (partialValue: Int128, overflow: Bool)

Returns the product of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func remainderReportingOverflow(dividingBy: Int128) -> (partialValue: Int128, overflow: Bool)

Returns the remainder after dividing this value by the given value, along with a Boolean value indicating whether overflow occurred during division.

func subtractingReportingOverflow(Int128) -> (partialValue: Int128, overflow: Bool)

Returns the difference obtained by subtracting the given value from this value, along with a Boolean value indicating whether overflow occurred in the operation.

### Type Properties

static var bitWidth: Int

The number of bits used for the underlying binary representation of values of this type.

static var max: Int128

The maximum representable integer in this type.

static var min: Int128

The minimum representable integer in this type.

### Type Methods

static func random(in: Range&lt;Self>) -> Self

Returns a random value within the specified range.

static func random(in: ClosedRange&lt;Self>) -> Self

Returns a random value within the specified range.

static func random&lt;T>(in: ClosedRange&lt;Self>, using: inout T) -> Self

Returns a random value within the specified range, using the given generator as a source for randomness.

static func random&lt;T>(in: Range&lt;Self>, using: inout T) -> Self

Returns a random value within the specified range, using the given generator as a source for randomness.

