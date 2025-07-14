

- Foundation
- FormatStyle
-  relative(presentation:unitsStyle:) 

Type Method

# relative(presentation:unitsStyle:)

Returns a style for formatting a date as relative to the current date.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func relative(
    presentation: Date.RelativeFormatStyle.Presentation,
    unitsStyle: Date.RelativeFormatStyle.UnitsStyle = .wide
) -> Self
```

Available when `Self` is `Date.RelativeFormatStyle`.

## Parameters 

`presentation`  

The style to use when describing a relative date; for example, “1 day ago” or “yesterday”.

`unitsStyle`  

The style to use when formatting the quantity or the name of the unit; for example, “1 day ago” or “one day ago”.

## Return Value

A relative date format style customized with the specified presentation and unit styles.

## Discussion

Use this static method when the call point allows the use of Date.RelativeFormatStyle. You typically do this when calling the formatted(_:) method of Date.

The following example shows the relative(presentation:unitsStyle:) relative format style with two different presentations.

```
if let past = Calendar.current.date(byAdding: .day, value: -7, to: Date()) {
    let formattedNumeric = past.formatted(
        .relative(presentation: .numeric)) // "1 week ago"
    let formattedNamed = past.formatted(
        .relative(presentation: .named)) // "last week"
}
```

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

struct RelativeFormatStyle

A format style that forms locale-aware string representations of a relative date or time.

static func components(style: Date.ComponentsFormatStyle.Style, fields: Set&lt;Date.ComponentsFormatStyle.Field>?) -> Self

Returns a style for formatting a date interval in terms of specific date components.

struct ComponentsFormatStyle

A style for formatting a date interval in terms of specific date components.

