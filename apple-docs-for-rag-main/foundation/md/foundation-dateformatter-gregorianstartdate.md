

- Foundation
- DateFormatter
-  gregorianStartDate 

Instance Property

# gregorianStartDate

The start date of the Gregorian calendar for the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var gregorianStartDate: Date? { get set }
```

## Discussion

This is used to specify the start date for the Gregorian calendar switch from the Julian calendar. Different locales switched at different times. Normally you should just accept the locale’s default date for the switch.

See NSCalendar for more information.

## See Also

### Managing Attributes

var calendar: Calendar!

The calendar for the receiver.

var defaultDate: Date?

The default date for the receiver.

var locale: Locale!

The locale for the receiver.

var timeZone: TimeZone!

The time zone for the receiver.

var twoDigitStartDate: Date?

The earliest date that can be denoted by a two-digit year specifier.

