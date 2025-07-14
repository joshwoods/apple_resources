

- Swift
- FloatingPointRoundingRule
-  FloatingPointRoundingRule.toNearestOrAwayFromZero 

Case

# FloatingPointRoundingRule.toNearestOrAwayFromZero

Round to the closest allowed value; if two values are equally close, the one with greater magnitude is chosen.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case toNearestOrAwayFromZero
```

## Discussion

This rounding rule is also known as “schoolbook rounding.” The following example shows the results of rounding numbers using this rule:

```
(5.2).rounded(.toNearestOrAwayFromZero)
// 5.0
(5.5).rounded(.toNearestOrAwayFromZero)
// 6.0
(-5.2).rounded(.toNearestOrAwayFromZero)
// -5.0
(-5.5).rounded(.toNearestOrAwayFromZero)
// -6.0
```

This rule is equivalent to the C `round` function and implements the `roundToIntegralTiesToAway` operation defined by the IEEE 754 specification.

