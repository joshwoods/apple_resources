

- Swift
- Double
-  isTotallyOrdered(belowOrEqualTo:) 

Instance Method

# isTotallyOrdered(belowOrEqualTo:)

Returns a Boolean value indicating whether this instance should precede or tie positions with the given value in an ascending sort.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isTotallyOrdered(belowOrEqualTo other: Self) -> Bool
```

## Parameters 

`other`  

A floating-point value to compare to this value.

## Return Value

`true` if this value is ordered below or the same as `other` in a total ordering of the floating-point type; otherwise, `false`.

## Discussion

This relation is a refinement of the less-than-or-equal-to operator (`

```
var numbers = [2.5, 21.25, 3.0, .nan, -9.5]
numbers.sort { !$1.isTotallyOrdered(belowOrEqualTo: $0) }
print(numbers)
// Prints "[-9.5, 2.5, 3.0, 21.25, nan]"
```

The `isTotallyOrdered(belowOrEqualTo:)` method implements the total order relation as defined by the IEEE 754 specification.

## See Also

### Comparing Values

Floating-Point Operators for Double

Perform arithmetic and bitwise operations or compare values.

func isEqual(to: Double) -> Bool

Returns a Boolean value indicating whether this instance is equal to the given value.

func isLess(than: Double) -> Bool

Returns a Boolean value indicating whether this instance is less than the given value.

func isLessThanOrEqualTo(Double) -> Bool

Returns a Boolean value indicating whether this instance is less than or equal to the given value.

static func minimum(Self, Self) -> Self

Returns the lesser of the two given values.

static func minimumMagnitude(Self, Self) -> Self

Returns the value with lesser magnitude.

static func maximum(Self, Self) -> Self

Returns the greater of the two given values.

static func maximumMagnitude(Self, Self) -> Self

Returns the value with greater magnitude.

