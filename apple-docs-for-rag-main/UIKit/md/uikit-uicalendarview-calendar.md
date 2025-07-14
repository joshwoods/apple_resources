

- UIKit
- UICalendarView
-  calendar 

Instance Property

# calendar

The calendar that the calendar view illustrates.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var calendar: Calendar { get set }
```

## Discussion

Defaults to current, which is the user’s current calendar set in Settings.

## See Also

### Setting calendar details

var locale: Locale

The locale the calendar view uses for calendar conventions.

var timeZone: TimeZone?

The time zone from the date the calendar view displays.

