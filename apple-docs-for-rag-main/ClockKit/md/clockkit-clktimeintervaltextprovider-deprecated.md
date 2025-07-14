

- ClockKit
-  CLKTimeIntervalTextProvider Deprecated

Class

# CLKTimeIntervalTextProvider

A formatted time range.

watchOS 2.0–9.0Deprecated

``` source
class CLKTimeIntervalTextProvider
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Creating a timeline entry

## Overview

This provider creates strings like “10:15–11:15AM” where the time range may span hours, days, or some larger time interval. The text provider takes into account the user’s region and locale settings.

Time interval strings are more appropriate in complication families where there’s sufficient space to draw the full time range, such as the modular large and utilitarian large families. In families where space is more limited, the provider may display only the start date of the time range.

When formatting the time interval, the time text provider drops the morning/evening indicator of the start time when it’s the same as the end time. Time intervals that are more than 24 hours are displayed as a range of days. The following are some examples of formatted time intervals:

- `9:30AM - 3:30PM`

- `9:30 - 10:30AM`

- `Jan 1 - Jan 7`

- `1/1 - 1/7`

## Topics

### Creating the Text Provider

convenience init(start: Date, end: Date)

Creates and returns a text provider with the specified start and end dates.

convenience init(start: Date, end: Date, timeZone: TimeZone?)

Creates and returns a text provider with the specified dates and time zone information.

### Getting the Time Information

var startDate: Date

The start date for the time interval.

var endDate: Date

The end date for the time interval.

var timeZone: TimeZone?

The time zone used to format time values.

## Relationships

### Inherits From

- CLKTextProvider

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Text providers

class CLKSimpleTextProvider

A single line of text to display in your complication interface.

Deprecated

class CLKDateTextProvider

A formatted string that conveys a date without any time information.

Deprecated

class CLKRelativeDateTextProvider

A formatted string that conveys the difference in time between the current date and a date that you specify.

Deprecated

class CLKTimeTextProvider

A formatted time value.

Deprecated

class CLKTextProvider

The common behavior for displaying text-based data in a complication.

Deprecated

