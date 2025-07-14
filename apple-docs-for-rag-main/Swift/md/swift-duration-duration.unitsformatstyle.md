

- Swift
- Duration
-  Duration.UnitsFormatStyle 

Structure

# Duration.UnitsFormatStyle

A format style that shows durations with localized labeled components

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct UnitsFormatStyle
```

## Overview

This style produces formatted strings that break out a duration’s individual components, like “2 min, 3 sec”.

Create a `UnitsFormatStyle` by providing a set of allowed Duration.UnitsFormatStyle.Unit instances — such as hours, minutes, or seconds — for formatted strings to include. You also specify a width for displaying these units, which controls whether they appear as full words (“minutes”) or abbreviations (“min”). The initializers also take optional parameters to control things like the handling of zero units and fractional parts. Then create a formatted string by calling formatted(_:) on a duration, passing the style, or format(_:) on the style, passing a duration. You can also use the style’s attributed property to create a style that produces AttributedString instances, which contains attributes that indicate the unit value of formatted runs of the string.

In situations that expect a Duration.UnitsFormatStyle, such as formatted(_:), you can use the convenience function `.units(allowed:width:maximumUnitCount:zeroValueUnits:valueLength:fractionalPart:)` to create a Duration.UnitsFormatStyle, rather than using the full initializer.

If you want to reuse a style to format many durations, call format(_:) on the style, passing in a new duration each time.

The following example creates `duration` to represent 1 hour, 10 minutes, 32 seconds, and 400 milliseconds. It then creates a Duration.UnitsFormatStyle to show the hours, minutes, seconds, and milliseconds parts, with a wide width that presents the full name of each unit.

```
let duration = Duration.seconds(70 * 60 + 32) + Duration.milliseconds(400)
let format = duration1.formatted(
     .units(allowed: [.hours, .minutes, .seconds, .milliseconds],
            width: .wide))
// format == "1 hour, 10 minutes, 32 seconds, 400 milliseconds"
```

The formatted string omits any units that aren’t needed to accurately represent the value. In the above example, a duration of exactly one minute would format as `1 minute`, omitting the hours, seconds, and milliseconds parts. To override this behavior and show the omitted units, use the initializer’s’ `zeroValueUnits` parameter.

## Topics

### Creating a units format style

init(allowedUnits: Set&lt;Duration.UnitsFormatStyle.Unit>, width: Duration.UnitsFormatStyle.UnitWidth, maximumUnitCount: Int?, zeroValueUnits: Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy, valueLength: Int?, fractionalPart: Duration.UnitsFormatStyle.FractionalPartDisplayStrategy)

Creates a units format style using the given parameters.

init&lt;ValueRange>(allowedUnits: Set&lt;Duration.UnitsFormatStyle.Unit>, width: Duration.UnitsFormatStyle.UnitWidth, maximumUnitCount: Int?, zeroValueUnits: Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy, valueLengthLimits: ValueRange, fractionalPart: Duration.UnitsFormatStyle.FractionalPartDisplayStrategy)

Creates a units format style using the given parameters.

### Formatting a duration

func format(Duration) -> String

Creates a locale-aware string representation from a duration value.

### Formatting a duration as an attributed string

var attributed: Duration.UnitsFormatStyle.Attributed

A property that formats the duration as an attributed string.

struct Attributed

A format style that formats durations as attributed strings.

### Working with units

var allowedUnits: Set&lt;Duration.UnitsFormatStyle.Unit>

The units that may be included in the output string.

struct Unit

A unit to use in formatting a duration.

var maximumUnitCount: Int?

The maximum number of time units to include in the output string.

var valueLengthLimits: Range&lt;Int>?

The padding or truncating behavior of the unit value.

### Working with unit widths

var unitWidth: Duration.UnitsFormatStyle.UnitWidth

The width of the unit and the spacing between the value and the unit.

struct UnitWidth

The width of a unit to use in formatting a duration.

### Working with zero values

var zeroValueUnitsDisplay: Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy

The strategy for how zero-value units are handled.

struct ZeroValueUnitsDisplayStrategy

A strategy that determines how to format a unit whose value is zero.

### Working with fractional values

var fractionalPartDisplay: Duration.UnitsFormatStyle.FractionalPartDisplayStrategy

The strategy for displaying a duration if it cannot be represented exactly with the allowed units.

struct FractionalPartDisplayStrategy

A strategy that determines how to format the fractional part of a duration if the allowed units can’t represent it exactly.

### Working with locales

var locale: Locale

The locale to use when formatting the duration.

func locale(Locale) -> Duration.UnitsFormatStyle

A modifier to set the locale of the format style.

## Relationships

### Conforms To

- Copyable
- Decodable
- DiscreteFormatStyle
- Encodable
- Equatable
- FormatStyle
- Hashable
- Sendable

## See Also

### Formatting a duration

func formatted() -> String

Formats the string using a localized hour-minute-second time pattern.

func formatted&lt;S>(S) -> S.FormatOutput

Formats the duration, using the provided format style.

struct TimeFormatStyle

A format style that shows durations in a compact, localized format with separators.

