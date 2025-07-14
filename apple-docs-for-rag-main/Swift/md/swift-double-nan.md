

- Swift
- Double
-  nan 

Type Property

# nan

A quiet NaN (“not a number”).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var nan: Double { get }
```

## Discussion

A NaN compares not equal, not greater than, and not less than every value, including itself. Passing a NaN to an operation generally results in NaN.

```
let x = 1.21
// x > Double.nan == false
// x 

Because a NaN always compares not equal to itself, to test whether a floating-point value is NaN, use its `isNaN` property instead of the equal-to operator (`==`). In the following example, `y` is NaN.

```
let y = x + Double.nan
print(y == Double.nan)
// Prints "false"
print(y.isNaN)
// Prints "true"
```

## See Also

### Accessing Numeric Constants

static var pi: Double

The mathematical constant pi (π), approximately equal to 3.14159.

static var infinity: Double

Positive infinity.

static var greatestFiniteMagnitude: Double

The greatest finite number representable by this type.

static var signalingNaN: Double

A signaling NaN (“not a number”).

static var ulpOfOne: Double

The unit in the last place of 1.0.

static var leastNonzeroMagnitude: Double

The least positive number.

static var leastNormalMagnitude: Double

The least positive normal number.

static var zero: Self

The zero value.

