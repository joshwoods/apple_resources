

- Foundation
- RelativeDateTimeFormatter
-  dateTimeStyle 

Instance Property

# dateTimeStyle

The style to use when describing a relative date, for example “yesterday” or “1 day ago”.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var dateTimeStyle: RelativeDateTimeFormatter.DateTimeStyle { get set }
```

## Discussion

Default is `numeric`.

```
let components = DateComponents(weekOfMonth: -1)
let formatter = RelativeDateTimeFormatter()
formatter.dateTimeStyle = .numeric
print(formatter.localizedString(from: components))
// Outputs:  1 week ago
```

To display relative dates using named styles, set this property to `named`.

```
let components = DateComponents(weekOfMonth: -1)
let formatter = RelativeDateTimeFormatter()
formatter.dateTimeStyle = .named
print(formatter.localizedString(from: components))
// Outputs:  last week
```

## See Also

### Configuring Formatter Options

var calendar: Calendar!

The calendar to use for formatting values that don’t have an inherent calendar of their own.

var locale: Locale!

The locale to use when formatting the date.

enum DateTimeStyle

A type that represents the style to use when formatting relative dates, such as “1 week ago” or “last week”.

var unitsStyle: RelativeDateTimeFormatter.UnitsStyle

The style to use when formatting the quantity or the name of the unit, such as “1 day ago” or “one day ago”.

enum UnitsStyle

A type that represents the style to use when formatting the units of relative dates.

var formattingContext: Formatter.Context

A description of where the formatted string will appear, allowing the formatter to capitalize the output appropriately.

