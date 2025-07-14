

- Swift
- Duration
- Duration.UnitsFormatStyle
- Duration.UnitsFormatStyle.FractionalPartDisplayStrategy
-  hide(rounded:) 

Type Method

# hide(rounded:)

Creates a display strategy that hides any fractional part rounding the unit value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func hide(rounded: FloatingPointRoundingRule = .toNearestOrEven) -> Duration.UnitsFormatStyle.FractionalPartDisplayStrategy
```

## See Also

### Using common strategies

static var hide: Duration.UnitsFormatStyle.FractionalPartDisplayStrategy

A display strategy that hides any fractional part by truncating it.

static func show(length: Int, rounded: FloatingPointRoundingRule, increment: Double?) -> Duration.UnitsFormatStyle.FractionalPartDisplayStrategy

Creates a display strategy that shows a fractional part.

