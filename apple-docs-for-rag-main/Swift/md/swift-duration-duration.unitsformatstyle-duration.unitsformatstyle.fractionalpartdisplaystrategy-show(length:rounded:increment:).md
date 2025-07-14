

- Swift
- Duration
- Duration.UnitsFormatStyle
- Duration.UnitsFormatStyle.FractionalPartDisplayStrategy
-  show(length:rounded:increment:) 

Type Method

# show(length:rounded:increment:)

Creates a display strategy that shows a fractional part.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func show(
    length: Int,
    rounded rule: FloatingPointRoundingRule = .toNearestOrEven,
    increment: Double? = nil
) -> Duration.UnitsFormatStyle.FractionalPartDisplayStrategy
```

## Parameters 

`length`  

The maximum string length of the fractional part.

`rule`  

A rule for rounding fractional values up or down. Defaults to FloatingPointRoundingRule.toNearestOrEven.

`increment`  

A multiple by which the formatter rounds the fractional part. The formatter produces a value that is an even multiple of this increment. If this parameter is `nil` (the default), the formatter doesn’t apply an increment. This value is only meaningful when the combination of allowed units, rounding rule, and formatting strategy requires expressing a unit with a fractional part. For example, a formatter that only allows minutes and uses a strategy with a length of `2` and default rounding rule formats 40 seconds as `0.67 minutes`. With a `increment` of `0.05`, the formatter formats this value as `0.65 minutes` instead.

## See Also

### Using common strategies

static var hide: Duration.UnitsFormatStyle.FractionalPartDisplayStrategy

A display strategy that hides any fractional part by truncating it.

static func hide(rounded: FloatingPointRoundingRule) -> Duration.UnitsFormatStyle.FractionalPartDisplayStrategy

Creates a display strategy that hides any fractional part rounding the unit value.

