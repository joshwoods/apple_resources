

- Foundation
- Date
-  Date.ComponentsFormatStyle 

Structure

# Date.ComponentsFormatStyle

A style for formatting a date interval in terms of specific date components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ComponentsFormatStyle
```

## Topics

### Structures

struct Field

struct Style

### Initializers

init(style: Date.ComponentsFormatStyle.Style, locale: Locale, calendar: Calendar, fields: Set&lt;Date.ComponentsFormatStyle.Field>?)

### Instance Properties

var calendar: Calendar

var fields: Set&lt;Date.ComponentsFormatStyle.Field>?

var isPositive: Bool

var locale: Locale

var style: Date.ComponentsFormatStyle.Style

### Instance Methods

func calendar(Calendar) -> Date.ComponentsFormatStyle

### Default Implementations

DiscreteFormatStyle Implementations

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

static func components(style: Date.ComponentsFormatStyle.Style, fields: Set&lt;Date.ComponentsFormatStyle.Field>?) -> Self

Returns a style for formatting a date interval in terms of specific date components.

