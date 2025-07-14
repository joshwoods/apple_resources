

- Swift
- FloatingPointRoundingRule
-  FloatingPointRoundingRule.up 

Case

# FloatingPointRoundingRule.up

Round to the closest allowed value that is greater than or equal to the source.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case up
```

## Discussion

The following example shows the results of rounding numbers using this rule:

```
(5.2).rounded(.up)
// 6.0
(5.5).rounded(.up)
// 6.0
(-5.2).rounded(.up)
// -5.0
(-5.5).rounded(.up)
// -5.0
```

This rule is equivalent to the C `ceil` function and implements the `roundToIntegralTowardPositive` operation defined by the IEEE 754 specification.

