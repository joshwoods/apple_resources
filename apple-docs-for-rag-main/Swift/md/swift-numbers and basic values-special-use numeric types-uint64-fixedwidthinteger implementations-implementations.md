

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Numbers and Basic Values
- Special-Use Numeric Types
- UInt64
-  FixedWidthInteger Implementations 

API Collection

# FixedWidthInteger Implementations

## Topics

### Operators

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

static func &amp;&lt;&lt; &lt;Other>(Self, Other) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width.

static func &amp;>> &lt;Other>(Self, Other) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width.

static func &amp;>> (UInt64, UInt64) -> UInt64

Returns the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width.

static func &amp;&lt;&lt; (Self, Self) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width.

static func &amp;&lt;&lt; (UInt64, UInt64) -> UInt64

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width.

static func &amp;>> (Self, Self) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width.

static func &amp;&lt;&lt;= &lt;Other>(inout Self, Other)

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

static func &amp;>>= &lt;Other>(inout Self, Other)

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

var littleEndian: Self

The little-endian representation of this integer.

### Type Methods

static func random(in: ClosedRange&lt;Self>) -> Self

Returns a random value within the specified range.

static func random(in: Range&lt;Self>) -> Self

Returns a random value within the specified range.

static func random&lt;T>(in: ClosedRange&lt;Self>, using: inout T) -> Self

Returns a random value within the specified range, using the given generator as a source for randomness.

static func random&lt;T>(in: Range&lt;Self>, using: inout T) -> Self

Returns a random value within the specified range, using the given generator as a source for randomness.

