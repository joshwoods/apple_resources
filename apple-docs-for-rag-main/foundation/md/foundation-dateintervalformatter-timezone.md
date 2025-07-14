

- Foundation
- DateIntervalFormatter
-  timeZone 

Instance Property

# timeZone

The time zone with which to specify time values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var timeZone: TimeZone! { get set }
```

## Discussion

The default value of this property is the default time zone for the current user, which is accessible from the default method of NSTimeZone. You can change this value to a different time zone to generate strings based on that time zone.

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

var locale: Locale!

The locale to use when formatting date and time values.

