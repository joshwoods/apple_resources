

- Swift
- Duration
- Duration.UnitsFormatStyle
- Duration.UnitsFormatStyle.FractionalPartDisplayStrategy
-  init(lengthLimits:roundingRule:roundingIncrement:) 

Initializer

# init(lengthLimits:roundingRule:roundingIncrement:)

Creates a fractional part display strategy that uses the provided behaviors.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    lengthLimits: Range,
    roundingRule: FloatingPointRoundingRule = .toNearestOrEven,
    roundingIncrement: Double? = nil
) where Range : RangeExpression, Range.Bound == Int
```

## Parameters 

`lengthLimits`  

The maximum string length of the fractional part.

`roundingRule`  

A rule for rounding fractional values up or down. Defaults to FloatingPointRoundingRule.toNearestOrEven.

`roundingIncrement`  

A multiple by which the formatter rounds the fractional part. The formatter produces a value that is an even multiple of this increment. If this parameter is `nil` (the default), the formatter doesn’t apply an increment. This value is only meaningful when the combination of allowed units, rounding rule, and formatting strategy requires expressing a unit with a fractional part. For example, a formatter that only allows minutes and uses a strategy with a length of `2` and default rounding rule formats 40 seconds as `0.67 minutes`. With a `roundingIncrement` of `0.05`, the formatter formats this value as `0.65 minutes` instead.

