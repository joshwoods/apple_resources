

- Swift
- Duration
- Duration.UnitsFormatStyle
- Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy
-  show(length:) 

Type Method

# show(length:)

Returns display strategy that shows leading fields whose value is zero, with a given number of digits.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func show(length: Int) -> Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy
```

## Parameters 

`length`  

The number of digits to show for zero-value units.

## See Also

### Using common strategies

static var hide: Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy

A display strategy that hides leading fields whose value is zero.

