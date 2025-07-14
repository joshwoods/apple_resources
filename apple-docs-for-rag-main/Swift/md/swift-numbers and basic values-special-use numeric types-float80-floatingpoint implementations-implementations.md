

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Numbers and Basic Values
- Special-Use Numeric Types
- Float80
-  FloatingPoint Implementations 

API Collection

# FloatingPoint Implementations

## Topics

### Operators

static func * (Float80, Float80) -> Float80

Multiplies two values and produces their product, rounding to a representable value.

static func *= (inout Float80, Float80)

Multiplies two values and stores the result in the left-hand-side variable, rounding to a representable value.

static func + (Float80, Float80) -> Float80

Adds two values and produces their sum, rounded to a representable value.

static func += (inout Float80, Float80)

Adds two values and stores the result in the left-hand-side variable, rounded to a representable value.

static func - (Float80) -> Float80

Calculates the additive inverse of a value.

static func - (Float80, Float80) -> Float80

Subtracts one value from another and produces their difference, rounded to a representable value.

static func -= (inout Float80, Float80)

Subtracts the second value from the first and stores the difference in the left-hand-side variable, rounding to a representable value.

static func / (Float80, Float80) -> Float80

Returns the quotient of dividing the first value by the second, rounded to a representable value.

static func > (Self, Self) -> Bool

static func /= (inout Float80, Float80)

Divides the first value by the second and stores the quotient in the left-hand-side variable, rounding to a representable value.

static func >= (Self, Self) -> Bool

static func &lt;= (Self, Self) -> Bool

### Initializers

init&lt;Source>(Source)

Creates a new value, rounded to the closest possible representation.

init(Int)

Creates a new value, rounded to the closest possible representation.

init?&lt;Source>(exactly: Source)

Creates a new value, if the given integer can be represented exactly.

init(sign: FloatingPointSign, exponent: Int, significand: Float80)

Creates a new value from the given sign, exponent, and significand.

init(signOf: Float80, magnitudeOf: Float80)

Creates a new floating-point value using the sign of one value and the magnitude of another.

init(signOf: Self, magnitudeOf: Self)

Creates a new floating-point value using the sign of one value and the magnitude of another.

### Instance Properties

var exponent: Int

The exponent of the floating-point value.

var floatingPointClass: FloatingPointClassification

The classification of this value.

var isCanonical: Bool

A Boolean value indicating whether the instance’s representation is in its canonical form.

var isFinite: Bool

A Boolean value indicating whether this instance is finite.

var isInfinite: Bool

A Boolean value indicating whether the instance is infinite.

var isNaN: Bool

A Boolean value indicating whether the instance is NaN (“not a number”).

var isNormal: Bool

A Boolean value indicating whether this instance is normal.

var isSignalingNaN: Bool

A Boolean value indicating whether the instance is a signaling NaN.

var isSubnormal: Bool

A Boolean value indicating whether the instance is subnormal.

var isZero: Bool

A Boolean value indicating whether the instance is equal to zero.

var nextDown: Self

The greatest representable value that compares less than this value.

var nextUp: Float80

The least representable value that compares greater than this value.

var sign: FloatingPointSign

The sign of the floating-point value.

var significand: Float80

The significand of the floating-point value.

var ulp: Float80

The unit in the last place of this value.

### Instance Methods

func addProduct(Float80, Float80)

Adds the product of the two given values to this value in place, computed without intermediate rounding.

func addingProduct(Self, Self) -> Self

Returns the result of adding the product of the two given values to this value, computed without intermediate rounding.

func formRemainder(dividingBy: Float80)

Replaces this value with the remainder of itself divided by the given value.

func formSquareRoot()

Replaces this value with its square root, rounded to a representable value.

func formTruncatingRemainder(dividingBy: Float80)

Replaces this value with the remainder of itself divided by the given value using truncating division.

func isEqual(to: Float80) -> Bool

Returns a Boolean value indicating whether this instance is equal to the given value.

func isLess(than: Float80) -> Bool

Returns a Boolean value indicating whether this instance is less than the given value.

func isLessThanOrEqualTo(Float80) -> Bool

Returns a Boolean value indicating whether this instance is less than or equal to the given value.

func isTotallyOrdered(belowOrEqualTo: Self) -> Bool

Returns a Boolean value indicating whether this instance should precede or tie positions with the given value in an ascending sort.

func negate()

Replaces this value with its additive inverse.

func remainder(dividingBy: Self) -> Self

Returns the remainder of this value divided by the given value.

func round()

func round(FloatingPointRoundingRule)

Rounds the value to an integral value using the specified rounding rule.

func rounded() -> Self

func rounded(FloatingPointRoundingRule) -> Self

Returns this value rounded to an integral value using the specified rounding rule.

func squareRoot() -> Self

Returns the square root of the value, rounded to a representable value.

func truncatingRemainder(dividingBy: Self) -> Self

Returns the remainder of this value divided by the given value using truncating division.

### Type Aliases

typealias Exponent

A type that can represent any written exponent.

### Type Properties

static var greatestFiniteMagnitude: Float80

The greatest finite number representable by this type.

static var infinity: Float80

Positive infinity.

static var leastNonzeroMagnitude: Float80

The least positive number.

static var leastNormalMagnitude: Float80

The least positive normal number.

static var nan: Float80

A quiet NaN (“not a number”).

static var pi: Float80

The mathematical constant pi (π), approximately equal to 3.14159.

static var radix: Int

The radix, or base of exponentiation, for a floating-point type.

static var signalingNaN: Float80

A signaling NaN (“not a number”).

static var ulpOfOne: Float80

The unit in the last place of 1.0.

static var ulpOfOne: Self

The unit in the last place of 1.0.

### Type Methods

static func maximum(Self, Self) -> Self

Returns the greater of the two given values.

static func maximumMagnitude(Self, Self) -> Self

Returns the value with greater magnitude.

static func minimum(Self, Self) -> Self

Returns the lesser of the two given values.

static func minimumMagnitude(Self, Self) -> Self

Returns the value with lesser magnitude.

