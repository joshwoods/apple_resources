

- Foundation
- DateIntervalFormatter
-  locale 

Instance Property

# locale

The locale to use when formatting date and time values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var locale: Locale! { get set }
```

## Discussion

The default value of this property is the current user’s locale, which is accessible from the current method of NSLocale. You can change this value to a different locale to generate strings based on that locale.

## See Also

### Configuring the Formatter Options

var dateStyle: DateIntervalFormatter.Style

The style to use when formatting day, month, and year information.

var timeStyle: DateIntervalFormatter.Style

The style to use when formatting hour, minute, and second information.

var dateTemplate: String!

The template for formatting one date and time value.

var calendar: Calendar!

The calendar to use for date values.

var timeZone: TimeZone!

The time zone with which to specify time values.

