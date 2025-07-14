

- Foundation
- RelativeDateTimeFormatter
-  RelativeDateTimeFormatter.UnitsStyle 

Enumeration

# RelativeDateTimeFormatter.UnitsStyle

A type that represents the style to use when formatting the units of relative dates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum UnitsStyle
```

## Topics

### Formatting Date and Time Units

case abbreviated

A style that uses abbreviated units, such as “2 mo. ago”.

case full

A style that uses full units, such as “2 months ago”.

case short

A style that uses shortened units, such as “2 mo. ago”.

case spellOut

A style that spells out units such as “two months ago”.

case abbreviated

A style that uses abbreviated units, such as “2 mo. ago”.

case full

A style that uses full units, such as “2 months ago”.

case short

A style that uses shortened units, such as “2 mo. ago”.

case spellOut

A style that spells out units such as “two months ago”.

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

enum DateTimeStyle

A type that represents the style to use when formatting relative dates, such as “1 week ago” or “last week”.

var unitsStyle: RelativeDateTimeFormatter.UnitsStyle

The style to use when formatting the quantity or the name of the unit, such as “1 day ago” or “one day ago”.

var formattingContext: Formatter.Context

A description of where the formatted string will appear, allowing the formatter to capitalize the output appropriately.

