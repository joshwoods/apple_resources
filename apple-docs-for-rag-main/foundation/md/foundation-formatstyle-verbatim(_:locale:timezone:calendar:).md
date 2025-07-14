

- Foundation
- FormatStyle
-  verbatim(\_:locale:timeZone:calendar:) 

Type Method

# verbatim(\_:locale:timeZone:calendar:)

Returns a style for formatting a date with an explicitly-specified style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func verbatim(
    _ format: Date.FormatString,
    locale: Locale? = nil,
    timeZone: TimeZone,
    calendar: Calendar
) -> Date.VerbatimFormatStyle
```

Available when `Self` is `Date.VerbatimFormatStyle`.

## Parameters 

`format`  

A Date.FormatString that provides the explicit components and their respective styles to use when formatting a date.

`locale`  

The locale to use when formatting. Defaults to `nil`.

`timeZone`  

The time zone to use when formatting.

`calendar`  

The calendar to use when formatting.

## Return Value

A date format style that uses the provided format string and timekeeping parameters.

## Discussion

Use this format style only when you need to produce or parse an exact format, such as when working with programmatically-produced date strings. For formatting dates that people read, use dateTime to get a localized Date.FormatStyle instead. To use the ISO-8601 standard, use iso8601 to get a Date.ISO8601FormatStyle.

Use the dot-notation form of this type method when the call point allows the use of Date.VerbatimFormatStyle. You typically do this when calling the formatted(_:) method of Date.

The following example formats the current date with a verbatim format that uses a two-digit month, two-digit day, and default-digits year, separated by slashes. The format style zero-pads the month and day components. This style isn’t localized — while this format string mimicks `en_US` conventions, it uses this format in any locale, ignoring locale-apporpriate conventions.

```
let date = Date()
let formatted = date.formatted(
    .verbatim("\(month: .twoDigits)/\(day: .twoDigits)/\(year: .defaultDigits)" as Date.FormatString,
              locale: .autoupdatingCurrent,
              timeZone: .current,
              calendar: .current)) // 12/05/2022
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

