

- Swift
- Float
-  maximumMagnitude(\_:\_:) 

Type Method

# maximumMagnitude(\_:\_:)

Returns the value with greater magnitude.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func maximumMagnitude(
    _ x: Self,
    _ y: Self
) -> Self
```

## Parameters 

`x`  

A floating-point value.

`y`  

Another floating-point value.

## Return Value

Whichever of `x` or `y` has greater magnitude, or whichever is a number if the other is NaN.

## Discussion

This method returns the value with greater magnitude of the two given values, preserving order and eliminating NaN when possible. For two values `x` and `y`, the result of `maximumMagnitude(x, y)` is `x` if `x.magnitude > y.magnitude`, `y` if `x.magnitude 

```
Double.maximumMagnitude(10.0, -25.0)
// -25.0
Double.maximumMagnitude(10.0, .nan)
// 10.0
Double.maximumMagnitude(.nan, -25.0)
// -25.0
Double.maximumMagnitude(.nan, .nan)
// nan
```

The `maximumMagnitude` method implements the `maxNumMag` operation defined by the IEEE 754 specification.

## See Also

### Comparing Values

Floating-Point Operators for Float

Perform arithmetic and bitwise operations or compare values.

func isEqual(to: Float) -> Bool

Returns a Boolean value indicating whether this instance is equal to the given value.

func isLess(than: Float) -> Bool

Returns a Boolean value indicating whether this instance is less than the given value.

func isLessThanOrEqualTo(Float) -> Bool

Returns a Boolean value indicating whether this instance is less than or equal to the given value.

func isTotallyOrdered(belowOrEqualTo: Self) -> Bool

Returns a Boolean value indicating whether this instance should precede or tie positions with the given value in an ascending sort.

static func maximum(Self, Self) -> Self

Returns the greater of the two given values.

static func minimum(Self, Self) -> Self

Returns the lesser of the two given values.

static func minimumMagnitude(Self, Self) -> Self

Returns the value with lesser magnitude.

