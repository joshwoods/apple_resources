

- Foundation
- RelativeDateTimeFormatter
-  RelativeDateTimeFormatter.DateTimeStyle 

Enumeration

# RelativeDateTimeFormatter.DateTimeStyle

A type that represents the style to use when formatting relative dates, such as “1 week ago” or “last week”.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum DateTimeStyle
```

## Topics

### Formatting Dates and Times

case named

A style that uses named styles to describe relative dates, such as “yesterday”, “last week”, or “next week”.

case numeric

A style that uses a numeric style to describe relative dates, such as “1 day ago” or “in 3 weeks”.

case named

A style that uses named styles to describe relative dates, such as “yesterday”, “last week”, or “next week”.

case numeric

A style that uses a numeric style to describe relative dates, such as “1 day ago” or “in 3 weeks”.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Formatter Options

var calendar: Calendar!

The calendar to use for formatting values that don’t have an inherent calendar of their own.

var locale: Locale!

The locale to use when formatting the date.

var dateTimeStyle: RelativeDateTimeFormatter.DateTimeStyle

The style to use when describing a relative date, for example “yesterday” or “1 day ago”.

var unitsStyle: RelativeDateTimeFormatter.UnitsStyle

The style to use when formatting the quantity or the name of the unit, such as “1 day ago” or “one day ago”.

enum UnitsStyle

A type that represents the style to use when formatting the units of relative dates.

var formattingContext: Formatter.Context

A description of where the formatted string will appear, allowing the formatter to capitalize the output appropriately.

