

- Foundation
- Date
-  Date.ISO8601FormatStyle 

Structure

# Date.ISO8601FormatStyle

A type that converts between dates and their ISO-8601 string representations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ISO8601FormatStyle
```

## Overview

The Date.ISO8601FormatStyle type generates and parses string representations of dates following the ISO-8601 standard, like `2024-04-01T12:34:56.789Z`. Use this type to create ISO-8601 representations of dates and create dates from text strings in ISO 8601 format. For other formatting conventions, like human-readable, localized date formats, use Date.FormatStyle.

Instance modifier methods applied to an ISO-8601 format style customize the formatted output, as the following example illustrates.

```
let now = Date()
print(now.formatted(Date.ISO8601FormatStyle().dateSeparator(.dash)))
// 2021-06-21T211015Z
```

Use the static factory property `iso8601-4m3gx` to create an instance of Date.ISO8601FormatStyle. Then apply instance modifier methods to customize the format, as in the example below.

```
let meetNow = Date()
let formatted = meetNow.formatted(.iso8601
    .year()
    .month()
    .day()
    .timeZone(separator: .omitted)
    .time(includingFractionalSeconds: true)
    .timeSeparator(.colon)
) // "2022-06-10T12:34:56.789Z"

```

## Topics

### Creating an ISO 8601 Format Style

init(dateSeparator: Date.ISO8601FormatStyle.DateSeparator, dateTimeSeparator: Date.ISO8601FormatStyle.DateTimeSeparator, timeZone: TimeZone)

Creates an instance using the provided date separator, date and time components separator, and time zone.

### Modifying an ISO 8601 Format Style

var dateSeparator: Date.ISO8601FormatStyle.DateSeparator

The character used to separate the components of a date.

var dateTimeSeparator: Date.ISO8601FormatStyle.DateTimeSeparator

The character used to separate the date and time components of an ISO 8601 string representation of a date.

var timeZone: TimeZone

The time zone used to create and parse date representations.

func dateTimeSeparator(Date.ISO8601FormatStyle.DateTimeSeparator) -> Date.ISO8601FormatStyle

Sets the character that specifies the date and time components.

### Modifying Dates in an ISO 8601 Format Style

func dateSeparator(Date.ISO8601FormatStyle.DateSeparator) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to use the specified date separator.

func year() -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the year in the formatted output.

func month() -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the month in the formatted output.

func weekOfYear() -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the week of the year in the formatted output.

func day() -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the day in the formatted output.

### Modifying Times in an ISO 8601 Format Style

func time(includingFractionalSeconds: Bool) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the time in the formatted output.

func timeSeparator(Date.ISO8601FormatStyle.TimeSeparator) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to use the specified time separator.

func timeZone(separator: Date.ISO8601FormatStyle.TimeZoneSeparator) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the time zone in the formatted output.

func timeZoneSeparator(Date.ISO8601FormatStyle.TimeZoneSeparator) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to use the specified time zone separator.

### Comparing ISO 8601 Format Styles

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Supporting Types

enum DateSeparator

A type describing the character separating year, month, and day components of a date in an ISO 8601 date format.

enum DateTimeSeparator

Type describing the character separating the date and time components of a date in an ISO 8601 date format.

enum TimeSeparator

Type describing the character separating the time components of a date in an ISO 8601 date format.

enum TimeZoneSeparator

A type describing the character separating the time and time zone of a date in an ISO 8601 date format.

### Initializers

init(dateSeparator: Date.ISO8601FormatStyle.DateSeparator, dateTimeSeparator: Date.ISO8601FormatStyle.DateTimeSeparator, timeSeparator: Date.ISO8601FormatStyle.TimeSeparator, timeZoneSeparator: Date.ISO8601FormatStyle.TimeZoneSeparator, includingFractionalSeconds: Bool, timeZone: TimeZone)

### Instance Properties

var includingFractionalSeconds: Bool

var timeSeparator: Date.ISO8601FormatStyle.TimeSeparator

var timeZoneSeparator: Date.ISO8601FormatStyle.TimeZoneSeparator

## Relationships

### Conforms To

- Copyable
- CustomConsumingRegexComponent
- Decodable
- Encodable
- Equatable
- FormatStyle
- Hashable
- ParseStrategy
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

