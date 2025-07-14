

- Foundation
- Locale
- Locale.Components
-  calendar 

Instance Property

# calendar

The calendar used by the locale.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var calendar: Calendar.Identifier?
```

## Discussion

Set this property to override the locale’s default calendar. To request the default calendar used by the locale, use the Locale property calendar.

This property corresponds to the `ca` key of the Unicode BCP 47 extension.

## See Also

### Specifying date and time components

enum Identifier

An enumeration for the available calendars.

var firstDayOfWeek: Locale.Weekday?

The first day of the week as represented by this locale.

enum Weekday

A type that represents weekdays, used for indicating a locale’s first day of the week.

var hourCycle: Locale.HourCycle?

The hour cycle used by the locale, like one-to-twelve or zero-to-twenty-three.

enum HourCycle

A type that represents the hour cycle used in a locale, like one-to-twelve or zero-to-twenty-three.

var timeZone: TimeZone?

The time zone used by the locale.

