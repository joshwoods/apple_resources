

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Numbers and Basic Values
- Special-Use Numeric Types
- UInt64
-  BinaryInteger Implementations 

API Collection

# BinaryInteger Implementations

## Topics

### Operators

static func != &lt;Other>(Self, Other) -> Bool

Returns a Boolean value indicating whether the two given values are not equal.

static func &amp; (UInt64, UInt64) -> UInt64

Returns the result of performing a bitwise AND operation on the two given values.

static func &amp; (Self, Self) -> Self

Returns the result of performing a bitwise AND operation on the two given values.

static func * (UInt64, UInt64) -> UInt64

Multiplies two values and produces their product.

static func + (UInt64, UInt64) -> UInt64

Adds two values and produces their sum.

static func - (UInt64, UInt64) -> UInt64

Subtracts one value from another and produces their difference.

static func == &lt;Other>(Self, Other) -> Bool

Returns a Boolean value indicating whether the two given values are equal.

static func ^ (Self, Self) -> Self

Returns the result of performing a bitwise XOR operation on the two given values.

static func | (Self, Self) -> Self

Returns the result of performing a bitwise OR operation on the two given values.

static func ^ (UInt64, UInt64) -> UInt64

Returns the result of performing a bitwise XOR operation on the two given values.

static func > (Self, Self) -> Bool

static func % (UInt64, UInt64) -> UInt64

Returns the remainder of dividing the first value by the second.

static func | (UInt64, UInt64) -> UInt64

Returns the result of performing a bitwise OR operation on the two given values.

static func &lt; &lt;Other>(Self, Other) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

static func / (UInt64, UInt64) -> UInt64

Returns the quotient of dividing the first value by the second.

static func > &lt;Other>(Self, Other) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than that of the second argument.

static func &lt;= &lt;Other>(Self, Other) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than or equal to that of the second argument.

static func &lt;= (Self, Self) -> Bool

static func >= &lt;Other>(Self, Other) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than or equal to that of the second argument.

static func >= (Self, Self) -> Bool

static func >> &lt;Other>(Self, Other) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the right.

static func &lt;&lt; &lt;Other>(Self, Other) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the left.

static func >> &lt;RHS>(Self, RHS) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the right.

static func &lt;&lt; &lt;RHS>(Self, RHS) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the left.

static func >>= &lt;Other>(inout Self, Other)

Stores the result of shifting a value’s binary representation the specified number of digits to the right in the left-hand-side variable.

static func &lt;&lt;= &lt;Other>(inout Self, Other)

Stores the result of shifting a value’s binary representation the specified number of digits to the left in the left-hand-side variable.

static func ~ (Self) -> Self

Returns the inverse of the bits set in the argument.

### Initializers

init()

Creates a new value equal to zero.

init(String, format: IntegerFormatStyle&lt;Self>, lenient: Bool) throws

init(String, format: IntegerFormatStyle&lt;Self>.Currency, lenient: Bool) throws

init(String, format: IntegerFormatStyle&lt;Self>.Percent, lenient: Bool) throws

init&lt;S>(S.ParseInput, strategy: S) throws

Initialize an instance by parsing `value` with the given `strategy`.

init&lt;S>(S.ParseInput, strategy: S) throws

Initialize an instance by parsing `value` with the given `strategy`.

init&lt;Other>(clamping: Other)

Creates a new instance with the representable value that’s closest to the given integer.

init&lt;T>(truncatingIfNeeded: T)

Creates a new instance from the bit pattern of the given instance by sign-extending or truncating to fit this type.

### Instance Properties

var bitWidth: Int

The number of bits in the current binary representation of this value.

var description: String

A textual representation of this value.

### Instance Methods

func advanced(by: Int) -> Self

Returns a value that is offset the specified distance from this value.

func distance(to: Self) -> Int

Returns the distance from this value to the given value, expressed as a stride.

func formatted() -> String

Format `self` using `IntegerFormatStyle()`

func formatted&lt;S>(S) -> S.FormatOutput

Format `self` with the given format.

func formatted&lt;S>(S) -> S.FormatOutput

Format `self` with the given format. `self` is first converted to `S.FormatInput` type, then format with the given format.

func isMultiple(of: Self) -> Bool

Returns `true` if this value is a multiple of the given value, and `false` otherwise.

func quotientAndRemainder(dividingBy: Self) -> (quotient: Self, remainder: Self)

Returns the quotient and remainder of this value divided by the given value.

