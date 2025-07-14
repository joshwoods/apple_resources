

- Foundation
- FormatStyle
-  timeDuration 

Type Property

# timeDuration

A style for formatting a duration expressed as a range of dates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var timeDuration: Date.ComponentsFormatStyle { get }
```

Available when `Self` is `Date.ComponentsFormatStyle`.

## Discussion

Use this type property when the call point allows the use of Date.FormatStyle. You typically do this when calling the formatted(_:) method of Date.

The following example creates a one hour, thirty-five minute range between two dates, then uses SELF to format this duration as a string.

```
let now = Date.now
let future = now.addingTimeInterval(95)
let dateRange = now..

To use the Swift Duration type rather than `Date`, use Duration.TimeFormatStyle or Duration.UnitsFormatStyle instead, and their corresponding static accessors, time(pattern:) and units(allowed:width:maximumUnitCount:zeroValueUnits:valueLength:fractionalPart:).

## See Also

### Applying duration styles

struct ComponentsFormatStyle

A style for formatting a date interval in terms of specific date components.

static func time(pattern: Duration.TimeFormatStyle.Pattern) -> Self

Returns a style for formatting a duration using a provided pattern.

static func units(allowed: Set&lt;Duration.UnitsFormatStyle.Unit>, width: Duration.UnitsFormatStyle.UnitWidth, maximumUnitCount: Int?, zeroValueUnits: Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy, valueLength: Int?, fractionalPart: Duration.UnitsFormatStyle.FractionalPartDisplayStrategy) -> Self

Returns a style for formatting a duration that uses the specified units.

static func units&lt;ValueRange>(allowed: Set&lt;Duration.UnitsFormatStyle.Unit>, width: Duration.UnitsFormatStyle.UnitWidth, maximumUnitCount: Int?, zeroValueUnits: Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy, valueLengthLimits: ValueRange, fractionalPart: Duration.UnitsFormatStyle.FractionalPartDisplayStrategy) -> Self

Returns a style for formatting a duration range that uses the specified units, with padding/truncating behavior defined as a range.

