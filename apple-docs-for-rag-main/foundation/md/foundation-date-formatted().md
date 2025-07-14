

- Foundation
- Date
-  formatted() 

Instance Method

# formatted()

Generates a locale-aware string representation of a date using the default date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func formatted() -> String
```

## Return Value

A string, formatted according to the default style.

## Discussion

Use the formatted() method to apply the default format style to a date, as in the following example:

```
let birthday = Date()
print(birthday.formatted())
// 6/4/2021, 2:24 PM
```

The default date format style uses the `numeric` date style and the `shortened` time style.

To customize the formatted measurement string, use either the formatted(_:) method and include a `Measurement.FormatStyle` or the formatted(date:time:) and include a date and time style.

For more information about formatting dates, see Date.FormatStyle.

## See Also

### Formatting a Date

func formatted(date: Date.FormatStyle.DateStyle, time: Date.FormatStyle.TimeStyle) -> String

Generates a locale-aware string representation of a date using specified date and time format styles.

func formatted&lt;F>(F) -> F.FormatOutput

Generates a locale-aware string representation of a date using the specified date format style.

struct FormatStyle

A structure that creates a locale-appropriate string representation of a date instance and converts strings of dates and times into date instances.

struct RelativeFormatStyle

A format style that forms locale-aware string representations of a relative date or time.

struct IntervalFormatStyle

A format style that creates string representations of date intervals.

func ISO8601Format(Date.ISO8601FormatStyle) -> String

Generates a locale-aware string representation of a date using the ISO 8601 date format.

struct ISO8601FormatStyle

A type that converts between dates and their ISO-8601 string representations.

