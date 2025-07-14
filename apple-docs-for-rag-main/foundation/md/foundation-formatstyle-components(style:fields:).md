

- Foundation
- FormatStyle
-  components(style:fields:) 

Type Method

# components(style:fields:)

Returns a style for formatting a date interval in terms of specific date components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func components(
    style: Date.ComponentsFormatStyle.Style,
    fields: Set? = nil
) -> Self
```

Available when `Self` is `Date.ComponentsFormatStyle`.

## Parameters 

`style`  

The style to use for the fields, such as abbreviated or narrow.

`fields`  

A set of date component fields to include in the formatted output.

## Return Value

A date format style that uses the specified style and fields.

## Discussion

Use this type method when the call point allows the use of Date.ComponentsFormatStyle. You typically do this when calling the formatted(_:) method of a `Range`.

The following example creates a 120-day date range, and then uses a Date.ComponentsFormatStyle to express this as a count of weeks and days:

```
let date = Date()
let futureDate = Calendar.current.date(byAdding: .day, value: 120, to: date)!
let interval = (date..

## See Also

### Applying date and time styles

static var dateTime: Date.FormatStyle

A style for formatting a date and time.

struct FormatStyle

A structure that creates a locale-appropriate string representation of a date instance and converts strings of dates and times into date instances.

static var iso8601: Date.ISO8601FormatStyle

A style for formatting a date in accordance with the ISO-8601 standard.

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

struct ComponentsFormatStyle

A style for formatting a date interval in terms of specific date components.

