

- Swift
- FloatingPointRoundingRule
-  FloatingPointRoundingRule.awayFromZero 

Case

# FloatingPointRoundingRule.awayFromZero

Round to the closest allowed value whose magnitude is greater than or equal to that of the source.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case awayFromZero
```

## Discussion

The following example shows the results of rounding numbers using this rule:

```
(5.2).rounded(.awayFromZero)
// 6.0
(5.5).rounded(.awayFromZero)
// 6.0
(-5.2).rounded(.awayFromZero)
// -6.0
(-5.5).rounded(.awayFromZero)
// -6.0
```

