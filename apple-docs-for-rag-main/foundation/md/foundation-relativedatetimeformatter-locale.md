

- Foundation
- RelativeDateTimeFormatter
-  locale 

Instance Property

# locale

The locale to use when formatting the date.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var locale: Locale! { get set }
```

## Discussion

The default value is autoupdatingCurrent. If you set this property to `nil`, the formatter resets to using autoupdatingCurrent.

## See Also

### Configuring Formatter Options

var calendar: Calendar!

The calendar to use for formatting values that don’t have an inherent calendar of their own.

var dateTimeStyle: RelativeDateTimeFormatter.DateTimeStyle

The style to use when describing a relative date, for example “yesterday” or “1 day ago”.

enum DateTimeStyle

A type that represents the style to use when formatting relative dates, such as “1 week ago” or “last week”.

var unitsStyle: RelativeDateTimeFormatter.UnitsStyle

The style to use when formatting the quantity or the name of the unit, such as “1 day ago” or “one day ago”.

enum UnitsStyle

A type that represents the style to use when formatting the units of relative dates.

var formattingContext: Formatter.Context

A description of where the formatted string will appear, allowing the formatter to capitalize the output appropriately.

