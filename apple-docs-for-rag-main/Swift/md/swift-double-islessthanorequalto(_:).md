

- Swift
- Double
-  isLessThanOrEqualTo(\_:) 

Instance Method

# isLessThanOrEqualTo(\_:)

Returns a Boolean value indicating whether this instance is less than or equal to the given value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isLessThanOrEqualTo(_ other: Double) -> Bool
```

## Parameters 

`other`  

The value to compare with this value.

## Return Value

`true` if `other` is greater than this value; otherwise, `false`. If either this value or `other` is NaN, the result of this method is `false`.

## Discussion

This method serves as the basis for the less-than-or-equal-to operator (`IEEE 754 specification.

## See Also

### Comparing Values

Floating-Point Operators for Double

Perform arithmetic and bitwise operations or compare values.

func isEqual(to: Double) -> Bool

Returns a Boolean value indicating whether this instance is equal to the given value.

func isLess(than: Double) -> Bool

Returns a Boolean value indicating whether this instance is less than the given value.

func isTotallyOrdered(belowOrEqualTo: Self) -> Bool

Returns a Boolean value indicating whether this instance should precede or tie positions with the given value in an ascending sort.

static func minimum(Self, Self) -> Self

Returns the lesser of the two given values.

static func minimumMagnitude(Self, Self) -> Self

Returns the value with lesser magnitude.

static func maximum(Self, Self) -> Self

Returns the greater of the two given values.

static func maximumMagnitude(Self, Self) -> Self

Returns the value with greater magnitude.

