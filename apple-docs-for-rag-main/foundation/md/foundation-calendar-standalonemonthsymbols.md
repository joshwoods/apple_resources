

- Foundation
- Calendar
-  standaloneMonthSymbols 

Instance Property

# standaloneMonthSymbols

A list of standalone months in this calendar, localized to the Calendar’s `locale`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var standaloneMonthSymbols: [String] { get }
```

## Discussion

For example, for English in the Gregorian calendar, returns `["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"]`.

Note

Stand-alone properties are for use in places like calendar headers. Non-stand-alone properties are for use in context (for example, “Saturday, November 12th”).

Note

By default, Calendars have no locale set. If you wish to receive a localized answer, be sure to set the `locale` property first - most likely to `Locale.autoupdatingCurrent`.

## See Also

### Getting Month Symbols

var monthSymbols: [String]

A list of months in this calendar, localized to the Calendar’s `locale`.

var shortMonthSymbols: [String]

A list of shorter-named months in this calendar, localized to the Calendar’s `locale`.

var veryShortMonthSymbols: [String]

A list of very-shortly-named months in this calendar, localized to the Calendar’s `locale`.

var shortStandaloneMonthSymbols: [String]

A list of shorter-named standalone months in this calendar, localized to the Calendar’s `locale`.

var veryShortStandaloneMonthSymbols: [String]

A list of very-shortly-named standalone months in this calendar, localized to the Calendar’s `locale`.

