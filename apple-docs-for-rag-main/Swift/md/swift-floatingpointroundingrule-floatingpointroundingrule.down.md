

- Swift
- FloatingPointRoundingRule
-  FloatingPointRoundingRule.down 

Case

# FloatingPointRoundingRule.down

Round to the closest allowed value that is less than or equal to the source.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case down
```

## Discussion

The following example shows the results of rounding numbers using this rule:

```
(5.2).rounded(.down)
// 5.0
(5.5).rounded(.down)
// 5.0
(-5.2).rounded(.down)
// -6.0
(-5.5).rounded(.down)
// -6.0
```

This rule is equivalent to the C `floor` function and implements the `roundToIntegralTowardNegative` operation defined by the IEEE 754 specification.

