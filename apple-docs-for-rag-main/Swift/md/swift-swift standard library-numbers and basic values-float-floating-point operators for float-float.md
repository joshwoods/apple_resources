

- Swift
- Swift Standard Library
- Numbers and Basic Values
- Float
-  Floating-Point Operators for Float 

API Collection

# Floating-Point Operators for Float

Perform arithmetic and bitwise operations or compare values.

## Topics

### Arithmetic

static func + (Float, Float) -> Float

Adds two values and produces their sum, rounded to a representable value.

static func - (Float, Float) -> Float

Subtracts one value from another and produces their difference, rounded to a representable value.

static func * (Float, Float) -> Float

Multiplies two values and produces their product, rounding to a representable value.

static func / (Float, Float) -> Float

Returns the quotient of dividing the first value by the second, rounded to a representable value.

### Arithmetic with Assignment

static func += (inout Float, Float)

Adds two values and stores the result in the left-hand-side variable, rounded to a representable value.

static func -= (inout Float, Float)

Subtracts the second value from the first and stores the difference in the left-hand-side variable, rounding to a representable value.

static func *= (inout Float, Float)

Multiplies two values and stores the result in the left-hand-side variable, rounding to a representable value.

static func /= (inout Float, Float)

Divides the first value by the second and stores the quotient in the left-hand-side variable, rounding to a representable value.

### Comparison

static func == (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func &lt; (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

static func &lt;= (Self, Self) -> Bool

static func > (Self, Self) -> Bool

static func >= (Self, Self) -> Bool

### Negation

static func - (Float) -> Float

Calculates the additive inverse of a value.

static func + (Self) -> Self

Returns the given number unchanged.

### Range Expressions

static func ..&lt; (Self) -> PartialRangeUpTo&lt;Self>

Returns a partial range up to, but not including, its upper bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

## See Also

### Performing Calculations

func addingProduct(Self, Self) -> Self

Returns the result of adding the product of the two given values to this value, computed without intermediate rounding.

func addProduct(Float, Float)

Adds the product of the two given values to this value in place, computed without intermediate rounding.

func squareRoot() -> Self

Returns the square root of the value, rounded to a representable value.

func formSquareRoot()

Replaces this value with its square root, rounded to a representable value.

func remainder(dividingBy: Self) -> Self

Returns the remainder of this value divided by the given value.

func formRemainder(dividingBy: Float)

Replaces this value with the remainder of itself divided by the given value.

func truncatingRemainder(dividingBy: Self) -> Self

Returns the remainder of this value divided by the given value using truncating division.

func formTruncatingRemainder(dividingBy: Float)

Replaces this value with the remainder of itself divided by the given value using truncating division.

func negate()

Replaces this value with its additive inverse.

