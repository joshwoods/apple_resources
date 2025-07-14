

- Foundation
- DateIntervalFormatter
-  timeStyle 

Instance Property

# timeStyle

The style to use when formatting hour, minute, and second information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var timeStyle: DateIntervalFormatter.Style { get set }
```

## Discussion

Set this property to an appropriate value before generating string values. The default value of this property is DateIntervalFormatter.Style.none.

## See Also

### Configuring the Formatter Options

var dateStyle: DateIntervalFormatter.Style

The style to use when formatting day, month, and year information.

var dateTemplate: String!

The template for formatting one date and time value.

var calendar: Calendar!

The calendar to use for date values.

var locale: Locale!

The locale to use when formatting date and time values.

var timeZone: TimeZone!

The time zone with which to specify time values.

