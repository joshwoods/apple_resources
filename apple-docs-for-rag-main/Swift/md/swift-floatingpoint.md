

- Swift
-  FloatingPoint 

Protocol

# FloatingPoint

A floating-point numeric type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol FloatingPoint : Hashable, SignedNumeric, Strideable where Self == Self.Magnitude
```

## Overview

Floating-point types are used to represent fractional numbers, like 5.5, 100.0, or 3.14159274. Each floating-point type has its own possible range and precision. The floating-point types in the standard library are `Float`, `Double`, and `Float80` where available.

Create new instances of floating-point types using integer or floating-point literals. For example:

```
let temperature = 33.2
let recordHigh = 37.5
```

The `FloatingPoint` protocol declares common arithmetic operations, so you can write functions and algorithms that work on any floating-point type. The following example declares a function that calculates the length of the hypotenuse of a right triangle given its two perpendicular sides. Because the `hypotenuse(_:_:)` function uses a generic parameter constrained to the `FloatingPoint` protocol, you can call it using any floating-point type.

```
func hypotenuse(_ a: T, _ b: T) -> T {
    return (a * a + b * b).squareRoot()
}

let (dx, dy) = (3.0, 4.0)
let distance = hypotenuse(dx, dy)
// distance == 5.0
```

Floating-point values are represented as a *sign* and a *magnitude*, where the magnitude is calculated using the type’s *radix* and the instance’s *significand* and *exponent*. This magnitude calculation takes the following form for a floating-point value `x` of type `F`, where `**` is exponentiation:

```
x.significand * (F.radix ** x.exponent)
```

Here’s an example of the number -8.5 represented as an instance of the `Double` type, which defines a radix of 2.

```
let y = -8.5
// y.sign == .minus
// y.significand == 1.0625
// y.exponent == 3

let magnitude = 1.0625 * Double(2 ** 3)
// magnitude == 8.5
```

Types that conform to the `FloatingPoint` protocol provide most basic (clause 5) operations of the IEEE 754 specification. The base, precision, and exponent range are not fixed in any way by this protocol, but it enforces the basic requirements of any IEEE 754 floating-point type.

# Additional Considerations

In addition to representing specific numbers, floating-point types also have special values for working with overflow and nonnumeric results of calculation.

## Infinity

Any value whose magnitude is so great that it would round to a value outside the range of representable numbers is rounded to *infinity*. For a type `F`, positive and negative infinity are represented as `F.infinity` and `-F.infinity`, respectively. Positive infinity compares greater than every finite value and negative infinity, while negative infinity compares less than every finite value and positive infinity. Infinite values with the same sign are equal to each other.

```
let values: [Double] = [10.0, 25.0, -10.0, .infinity, -.infinity]
print(values.sorted())
// Prints "[-inf, -10.0, 10.0, 25.0, inf]"
```

Operations with infinite values follow real arithmetic as much as possible: Adding or subtracting a finite value, or multiplying or dividing infinity by a nonzero finite value, results in infinity.

## NaN (“not a number”)

Floating-point types represent values that are neither finite numbers nor infinity as NaN, an abbreviation for “not a number.” Comparing a NaN with any value, including another NaN, results in `false`.

```
let myNaN = Double.nan
print(myNaN > 0)
// Prints "false"
print(myNaN 

Because testing whether one NaN is equal to another NaN results in `false`, use the `isNaN` property to test whether a value is NaN.

```
print(myNaN.isNaN)
// Prints "true"
```

NaN propagates through many arithmetic operations. When you are operating on many values, this behavior is valuable because operations on NaN simply forward the value and don’t cause runtime errors. The following example shows how NaN values operate in different contexts.

Imagine you have a set of temperature data for which you need to report some general statistics: the total number of observations, the number of valid observations, and the average temperature. First, a set of observations in Celsius is parsed from strings to `Double` values:

```
let temperatureData = ["21.5", "19.25", "27", "no data", "28.25", "no data", "23"]
let tempsCelsius = temperatureData.map { Double($0) ?? .nan }
print(tempsCelsius)
// Prints "[21.5, 19.25, 27, nan, 28.25, nan, 23.0]"
```

Note that some elements in the `temperatureData ` array are not valid numbers. When these invalid strings are parsed by the `Double` failable initializer, the example uses the nil-coalescing operator (`??`) to provide NaN as a fallback value.

Next, the observations in Celsius are converted to Fahrenheit:

```
let tempsFahrenheit = tempsCelsius.map { $0 * 1.8 + 32 }
print(tempsFahrenheit)
// Prints "[70.7, 66.65, 80.6, nan, 82.85, nan, 73.4]"
```

The NaN values in the `tempsCelsius` array are propagated through the conversion and remain NaN in `tempsFahrenheit`.

Because calculating the average of the observations involves combining every value of the `tempsFahrenheit` array, any NaN values cause the result to also be NaN, as seen in this example:

```
let badAverage = tempsFahrenheit.reduce(0.0, +) / Double(tempsFahrenheit.count)
// badAverage.isNaN == true
```

Instead, when you need an operation to have a specific numeric result, filter out any NaN values using the `isNaN` property.

```
let validTemps = tempsFahrenheit.filter { !$0.isNaN }
let average = validTemps.reduce(0.0, +) / Double(validTemps.count)
```

Finally, report the average temperature and observation counts:

```
print("Average: \(average)°F in \(validTemps.count) " +
      "out of \(tempsFahrenheit.count) observations.")
// Prints "Average: 74.84°F in 5 out of 7 observations."
```

## Topics

### Operators

static func * (Self, Self) -> Self

Multiplies two values and produces their product, rounding to a representable value.

**Required**

static func *= (inout Self, Self)

Multiplies two values and stores the result in the left-hand-side variable, rounding to a representable value.

**Required**

static func + (Self, Self) -> Self

Adds two values and produces their sum, rounded to a representable value.

**Required**

static func += (inout Self, Self)

Adds two values and stores the result in the left-hand-side variable, rounded to a representable value.

**Required**

static func - (Self) -> Self

Calculates the additive inverse of a value.

**Required**

static func - (Self, Self) -> Self

Subtracts one value from another and produces their difference, rounded to a representable value.

**Required**

static func -= (inout Self, Self)

Subtracts the second value from the first and stores the difference in the left-hand-side variable, rounding to a representable value.

**Required**

static func / (Self, Self) -> Self

Returns the quotient of dividing the first value by the second, rounded to a representable value.

**Required**

static func /= (inout Self, Self)

Divides the first value by the second and stores the quotient in the left-hand-side variable, rounding to a representable value.

**Required**

### Associated Types

associatedtype Exponent : SignedInteger

A type that can represent any written exponent.

**Required**

### Initializers

init&lt;Source>(Source)

Creates a new value, rounded to the closest possible representation.

**Required** Default implementations provided.

init(Int)

Creates a new value, rounded to the closest possible representation.

**Required** Default implementations provided.

init?&lt;Source>(exactly: Source)

Creates a new value, if the given integer can be represented exactly.

**Required** Default implementations provided.

init(sign: FloatingPointSign, exponent: Self.Exponent, significand: Self)

Creates a new value from the given sign, exponent, and significand.

**Required**

init(signOf: Self, magnitudeOf: Self)

Creates a new floating-point value using the sign of one value and the magnitude of another.

**Required** Default implementation provided.

### Instance Properties

var exponent: Self.Exponent

The exponent of the floating-point value.

**Required**

var floatingPointClass: FloatingPointClassification

The classification of this value.

**Required** Default implementation provided.

var isCanonical: Bool

A Boolean value indicating whether the instance’s representation is in its canonical form.

**Required**

var isFinite: Bool

A Boolean value indicating whether this instance is finite.

**Required**

var isInfinite: Bool

A Boolean value indicating whether the instance is infinite.

**Required**

var isNaN: Bool

A Boolean value indicating whether the instance is NaN (“not a number”).

**Required**

var isNormal: Bool

A Boolean value indicating whether this instance is normal.

**Required**

var isSignalingNaN: Bool

A Boolean value indicating whether the instance is a signaling NaN.

**Required**

var isSubnormal: Bool

A Boolean value indicating whether the instance is subnormal.

**Required**

var isZero: Bool

A Boolean value indicating whether the instance is equal to zero.

**Required**

var nextDown: Self

The greatest representable value that compares less than this value.

**Required** Default implementation provided.

var nextUp: Self

The least representable value that compares greater than this value.

**Required**

var sign: FloatingPointSign

The sign of the floating-point value.

**Required**

var significand: Self

The significand of the floating-point value.

**Required**

var ulp: Self

The unit in the last place of this value.

**Required**

### Instance Methods

func addProduct(Self, Self)

Adds the product of the two given values to this value in place, computed without intermediate rounding.

**Required**

func addingProduct(Self, Self) -> Self

Returns the result of adding the product of the two given values to this value, computed without intermediate rounding.

**Required** Default implementation provided.

func formRemainder(dividingBy: Self)

Replaces this value with the remainder of itself divided by the given value.

**Required**

func formSquareRoot()

Replaces this value with its square root, rounded to a representable value.

**Required**

func formTruncatingRemainder(dividingBy: Self)

Replaces this value with the remainder of itself divided by the given value using truncating division.

**Required**

func isEqual(to: Self) -> Bool

Returns a Boolean value indicating whether this instance is equal to the given value.

**Required**

func isLess(than: Self) -> Bool

Returns a Boolean value indicating whether this instance is less than the given value.

**Required**

func isLessThanOrEqualTo(Self) -> Bool

Returns a Boolean value indicating whether this instance is less than or equal to the given value.

**Required**

func isTotallyOrdered(belowOrEqualTo: Self) -> Bool

Returns a Boolean value indicating whether this instance should precede or tie positions with the given value in an ascending sort.

**Required** Default implementation provided.

func negate()

Replaces this value with its additive inverse.

**Required**

func remainder(dividingBy: Self) -> Self

Returns the remainder of this value divided by the given value.

**Required** Default implementation provided.

func round()

func round(FloatingPointRoundingRule)

Rounds the value to an integral value using the specified rounding rule.

**Required**

func rounded() -> Self

func rounded(FloatingPointRoundingRule) -> Self

Returns this value rounded to an integral value using the specified rounding rule.

**Required** Default implementation provided.

func squareRoot() -> Self

Returns the square root of the value, rounded to a representable value.

**Required** Default implementation provided.

func truncatingRemainder(dividingBy: Self) -> Self

Returns the remainder of this value divided by the given value using truncating division.

**Required** Default implementation provided.

### Type Properties

static var greatestFiniteMagnitude: Self

The greatest finite number representable by this type.

**Required**

static var infinity: Self

Positive infinity.

**Required**

static var leastNonzeroMagnitude: Self

The least positive number.

**Required**

static var leastNormalMagnitude: Self

The least positive normal number.

**Required**

static var nan: Self

A quiet NaN (“not a number”).

**Required**

static var pi: Self

The mathematical constant pi (π), approximately equal to 3.14159.

**Required**

static var radix: Int

The radix, or base of exponentiation, for a floating-point type.

**Required** Default implementation provided.

static var signalingNaN: Self

A signaling NaN (“not a number”).

**Required**

static var ulpOfOne: Self

The unit in the last place of 1.0.

**Required** Default implementation provided.

### Type Methods

static func maximum(Self, Self) -> Self

Returns the greater of the two given values.

**Required** Default implementation provided.

static func maximumMagnitude(Self, Self) -> Self

Returns the value with greater magnitude.

**Required** Default implementation provided.

static func minimum(Self, Self) -> Self

Returns the lesser of the two given values.

**Required** Default implementation provided.

static func minimumMagnitude(Self, Self) -> Self

Returns the value with lesser magnitude.

**Required** Default implementation provided.

## Relationships

### Inherits From

- AdditiveArithmetic
- Comparable
- Equatable
- ExpressibleByIntegerLiteral
- Hashable
- Numeric
- SignedNumeric
- Strideable

### Inherited By

- BinaryFloatingPoint

### Conforming Types

- Double
- Float
- Float16
- Float80

## See Also

### Floating Point

protocol BinaryFloatingPoint

A radix-2 (binary) floating-point type.

