

- Foundation
- Locale
- Locale.Components
-  timeZone 

Instance Property

# timeZone

The time zone used by the locale.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var timeZone: TimeZone?
```

## Discussion

Set this value to specify a time zone associated with the locale.

This property corresponds to the `tz` key of the Unicode BCP 47 extension.

## See Also

### Specifying date and time components

var calendar: Calendar.Identifier?

The calendar used by the locale.

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

