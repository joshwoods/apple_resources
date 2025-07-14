

- Core Media
- CMTimeRoundingMethod
-  CMTimeRoundingMethod.quickTime 

Case

# CMTimeRoundingMethod.quickTime

Rounds using the QuickTime method.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
case quickTime
```

## Discussion

This method uses CMTimeRoundingMethod.roundTowardZero if converting from larger to smaller scale (more precision to less precision), but uses CMTimeRoundingMethod.roundAwayFromZero if converting from smaller to larger scale (less precision to more precision).

This method never rounds a negative number down to `0`, but instead returns the smallest magnitude negative time (`-1 / newTimescale`).

## See Also

### Rounding Methods

case roundHalfAwayFromZero

Rounds half away from zero.

case roundAwayFromZero

Rounds away from zero.

case roundTowardZero

Rounds toward zero.

case roundTowardPositiveInfinity

Rounds toward positive infinity.

case roundTowardNegativeInfinity

Rounds toward negative infinity.

