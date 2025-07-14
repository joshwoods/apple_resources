

- Swift
- Duration
- Duration.UnitsFormatStyle
- Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy
-  hide 

Type Property

# hide

A display strategy that hides leading fields whose value is zero.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var hide: Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy { get }
```

## See Also

### Using common strategies

static func show(length: Int) -> Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy

Returns display strategy that shows leading fields whose value is zero, with a given number of digits.

