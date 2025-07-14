

- Foundation
- DateFormatter
-  twoDigitStartDate 

Instance Property

# twoDigitStartDate

The earliest date that can be denoted by a two-digit year specifier.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var twoDigitStartDate: Date? { get set }
```

## Discussion

If the two-digit start date is set to January 6, 1976, then “January 1, 76” is interpreted as New Year’s Day in 2076, whereas “February 14, 76” is interpreted as Valentine’s Day in 1976.

By default, this property is equal to December 31, 1949.

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

var gregorianStartDate: Date?

The start date of the Gregorian calendar for the receiver.

