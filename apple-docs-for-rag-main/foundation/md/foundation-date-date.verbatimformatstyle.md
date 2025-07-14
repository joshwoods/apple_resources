

- Foundation
- Date
-  Date.VerbatimFormatStyle 

Structure

# Date.VerbatimFormatStyle

A style that formats a date with an explicitly-specified style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct VerbatimFormatStyle
```

## Topics

### Structures

struct Attributed

### Initializers

init(format: Date.FormatString, locale: Locale?, timeZone: TimeZone, calendar: Calendar)

### Instance Properties

var attributed: Date.AttributedStyleDeprecated

var attributedStyle: Date.VerbatimFormatStyle.Attributed

var calendar: Calendar

var locale: Locale?

var timeZone: TimeZone

## Relationships

### Conforms To

- Copyable
- CustomConsumingRegexComponent
- Decodable
- DiscreteFormatStyle
- Encodable
- Equatable
- FormatStyle
- Hashable
- ParseableFormatStyle
- RegexComponent
- Sendable

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

