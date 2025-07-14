

- Foundation
- FormatStyle
-  iso8601 

Type Property

# iso8601

A style for formatting a date in accordance with the ISO-8601 standard.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var iso8601: Date.ISO8601FormatStyle { get }
```

Available when `Self` is `Date.ISO8601FormatStyle`.

## Discussion

This style uses the ISO-8601 standard for formatting dates, such as `2024-04-01T12:34:56.789Z`. This style is well-suited for machine-readable date formatting. For other formatting conventions, like human-readable, localized date formats, use Date.FormatStyle.

Use this type property when the call point allows the use of Date.ISO8601FormatStyle. You typically do this when calling the formatted(_:) method of Date.

Customize the ISO-8601 date format style using modifier syntax to include or omit the various components of the date and time. For example:

```
let meetNow = Date()
let formatted = meetNow.formatted(
    .iso8601
    .year()
    .month()
    .day()
    .timeZone(separator: .omitted)
    .time(includingFractionalSeconds: true)
    .timeSeparator(.colon)
) // "2022-06-10T12:34:56.789Z"
```

## See Also

### Applying date and time styles

static var dateTime: Date.FormatStyle

A style for formatting a date and time.

struct FormatStyle

A structure that creates a locale-appropriate string representation of a date instance and converts strings of dates and times into date instances.

struct ISO8601FormatStyle

A type that converts between dates and their ISO-8601 string representations.

static func verbatim(Date.FormatString, locale: Locale?, timeZone: TimeZone, calendar: Calendar) -> Date.VerbatimFormatStyle

Returns a style for formatting a date with an explicitly-specified style.

struct VerbatimFormatStyle

A style that formats a date with an explicitly-specified style.

static var interval: Date.IntervalFormatStyle

A style for formatting a date interval.

struct IntervalFormatStyle

A format style that creates string representations of date intervals.

static func relative(presentation: Date.RelativeFormatStyle.Presentation, unitsStyle: Date.RelativeFormatStyle.UnitsStyle) -> Self

Returns a style for formatting a date as relative to the current date.

struct RelativeFormatStyle

A format style that forms locale-aware string representations of a relative date or time.

static func components(style: Date.ComponentsFormatStyle.Style, fields: Set&lt;Date.ComponentsFormatStyle.Field>?) -> Self

Returns a style for formatting a date interval in terms of specific date components.

struct ComponentsFormatStyle

A style for formatting a date interval in terms of specific date components.

