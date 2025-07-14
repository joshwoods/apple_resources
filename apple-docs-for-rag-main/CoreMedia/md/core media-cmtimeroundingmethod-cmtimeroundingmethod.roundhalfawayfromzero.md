

- Core Media
- CMTimeRoundingMethod
-  CMTimeRoundingMethod.roundHalfAwayFromZero 

Case

# CMTimeRoundingMethod.roundHalfAwayFromZero

Rounds half away from zero.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
case roundHalfAwayFromZero
```

## Discussion

This method rounds toward zero if the absolute value is less than `0.5`, and away from `0` if it’s greater than or equal to `0.5`.

This is the default rounding method.

## See Also

### Rounding Methods

case roundAwayFromZero

Rounds away from zero.

case roundTowardZero

Rounds toward zero.

case quickTime

Rounds using the QuickTime method.

case roundTowardPositiveInfinity

Rounds toward positive infinity.

case roundTowardNegativeInfinity

Rounds toward negative infinity.

