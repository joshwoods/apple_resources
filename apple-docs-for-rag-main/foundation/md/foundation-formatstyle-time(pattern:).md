

- Foundation
- FormatStyle
-  time(pattern:) 

Type Method

# time(pattern:)

Returns a style for formatting a duration using a provided pattern.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func time(pattern: Duration.TimeFormatStyle.Pattern) -> Self
```

Available when `Self` is `Duration.TimeFormatStyle`.

## Parameters 

`pattern`  

A Duration.TimeFormatStyle.Pattern that specifies the units to include in the displayed string and the behavior of the units.

## Return Value

A duration time format style customized with the specified pattern.

## Discussion

Use the dot-notation form of this type method when the call point allows the use of Duration.TimeFormatStyle. You typically do this when calling the formatted(_:) method of Duration.

The following example creates a duration to represent 1 hour, 10 minutes, 32 seconds, and 400 milliseconds. It then uses time(pattern:) to customize a Duration.TimeFormatStyle to show hours, minutes, and seconds, padding the hours part to two digits and limiting the fractional seconds to two digits. When used with the formatted(_:) method, the resulting string is `01:10:32.40`.

```
let duration = Duration.seconds(70 * 60 + 32) + Duration.milliseconds(400)
let format = duration.formatted(
    .time(pattern: .hourMinuteSecond(padHourToLength: 2,
                                     fractionalSecondsLength: 2)))
// format == "01:10:32.40"
```

## See Also

### Applying duration styles

static var timeDuration: Date.ComponentsFormatStyle

A style for formatting a duration expressed as a range of dates.

struct ComponentsFormatStyle

A style for formatting a date interval in terms of specific date components.

static func units(allowed: Set&lt;Duration.UnitsFormatStyle.Unit>, width: Duration.UnitsFormatStyle.UnitWidth, maximumUnitCount: Int?, zeroValueUnits: Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy, valueLength: Int?, fractionalPart: Duration.UnitsFormatStyle.FractionalPartDisplayStrategy) -> Self

Returns a style for formatting a duration that uses the specified units.

static func units&lt;ValueRange>(allowed: Set&lt;Duration.UnitsFormatStyle.Unit>, width: Duration.UnitsFormatStyle.UnitWidth, maximumUnitCount: Int?, zeroValueUnits: Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy, valueLengthLimits: ValueRange, fractionalPart: Duration.UnitsFormatStyle.FractionalPartDisplayStrategy) -> Self

Returns a style for formatting a duration range that uses the specified units, with padding/truncating behavior defined as a range.

