

- Foundation
- Calendar
-  veryShortStandaloneWeekdaySymbols 

Instance Property

# veryShortStandaloneWeekdaySymbols

A list of very-shortly-named weekdays in this calendar, localized to the Calendar’s `locale`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var veryShortStandaloneWeekdaySymbols: [String] { get }
```

## Discussion

For example, for English in the Gregorian calendar, returns `["S", "M", "T", "W", "T", "F", "S"]`.

Note

Stand-alone properties are for use in places like calendar headers. Non-stand-alone properties are for use in context (for example, “Saturday, November 12th”).

Note

By default, Calendars have no locale set. If you wish to receive a localized answer, be sure to set the `locale` property first - most likely to `Locale.autoupdatingCurrent`.

## See Also

### Getting Weekday Symbols

var weekdaySymbols: [String]

A list of weekdays in this calendar, localized to the Calendar’s `locale`.

var shortWeekdaySymbols: [String]

A list of shorter-named weekdays in this calendar, localized to the Calendar’s `locale`.

var veryShortWeekdaySymbols: [String]

A list of very-shortly-named weekdays in this calendar, localized to the Calendar’s `locale`.

var standaloneWeekdaySymbols: [String]

A list of standalone weekday names in this calendar, localized to the Calendar’s `locale`.

var shortStandaloneWeekdaySymbols: [String]

A list of shorter-named standalone weekdays in this calendar, localized to the Calendar’s `locale`.

