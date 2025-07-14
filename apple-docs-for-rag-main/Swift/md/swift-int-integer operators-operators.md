

- Swift
- Int
-  Integer Operators 

API Collection

# Integer Operators

Perform arithmetic and bitwise operations or compare values.

## Topics

### Arithmetic

static func + (Int, Int) -> Int

Adds two values and produces their sum.

static func - (Int, Int) -> Int

Subtracts one value from another and produces their difference.

static func * (Int, Int) -> Int

Multiplies two values and produces their product.

static func / (Int, Int) -> Int

Returns the quotient of dividing the first value by the second.

### Arithmetic with Assignment

static func += (inout Int, Int)

Adds two values and stores the result in the left-hand-side variable.

static func *= (inout Int, Int)

Multiplies two values and stores the result in the left-hand-side variable.

static func /= (inout Int, Int)

Divides the first value by the second and stores the quotient in the left-hand-side variable.

### Masked Arithmetic

static func &amp;+ (Self, Self) -> Self

Returns the sum of the two given values, wrapping the result in case of any overflow.

static func &amp;- (Self, Self) -> Self

Returns the difference of the two given values, wrapping the result in case of any overflow.

static func &amp;* (Self, Self) -> Self

Returns the product of the two given values, wrapping the result in case of any overflow.

static func &amp;+= (inout Self, Self)

Adds two values and stores the result in the left-hand-side variable, wrapping any overflow.

static func &amp;-= (inout Self, Self)

Subtracts the second value from the first and stores the difference in the left-hand-side variable, wrapping any overflow.

static func &amp;*= (inout Self, Self)

Multiplies two values and stores the result in the left-hand-side variable, wrapping any overflow.

### Bitwise Operations

static func &amp; (Int, Int) -> Int

Returns the result of performing a bitwise AND operation on the two given values.

static func &amp;= (inout Int, Int)

Stores the result of performing a bitwise AND operation on the two given values in the left-hand-side variable.

static func ~ (Self) -> Self

Returns the inverse of the bits set in the argument.

### Negation

static func - (Self) -> Self

Returns the additive inverse of the specified value.

static func + (Self) -> Self

Returns the given number unchanged.

### Comparison

static func == (Int, Int) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func == &lt;Other>(Self, Other) -> Bool

Returns a Boolean value indicating whether the two given values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func != &lt;Other>(Self, Other) -> Bool

Returns a Boolean value indicating whether the two given values are not equal.

### Range Expressions

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

### Deprecated

static func -= (inout Int, Int)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

## See Also

### Performing Calculations

func negate()

Replaces this value with its additive inverse.

func quotientAndRemainder(dividingBy: Self) -> (quotient: Self, remainder: Self)

Returns the quotient and remainder of this value divided by the given value.

func isMultiple(of: Self) -> Bool

Returns `true` if this value is a multiple of the given value, and `false` otherwise.

