

- ClockKit
-  CLKRelativeDateTextProvider Deprecated

Class

# CLKRelativeDateTextProvider

A formatted string that conveys the difference in time between the current date and a date that you specify.

watchOS 2.0–9.0Deprecated

``` source
class CLKRelativeDateTextProvider
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Creating a timeline entry

## Overview

You use a relative date text provider to implement timers or other relative time values in an efficient way. Instead of using multiple timeline entries to replicate a countdown timer, create a single timeline entry with a relative date text provider. When the user views the clock face, ClockKit automatically updates the relative time value in your complication, providing up-to-date time information.

When creating the formatted string, the relative date text provider creates the longest string that fits in the given space. It includes as many of the requested date elements as it can, but may truncate elements or use abbreviations as needed. The formatted string takes into account the user’s region and locale settings.

### Date Format Options

When creating a `CLKRelativeDateTextProvider` object, you must specify which calendar units you want included in the resulting date. Only the following calendar units are supported:

- NSYearCalendarUnit

- NSMonthCalendarUnit

- NSWeekOfMonthCalendarUnit

- NSDayCalendarUnit

- NSHourCalendarUnit

- NSMinuteCalendarUnit

- NSSecondCalendarUnit

Note

When creating a relative date provider using the CLKRelativeDateStyle.timer style, only the NSHourCalendarUnit, NSMinuteCalendarUnit, and NSSecondCalendarUnit units are supported.

All other calendar units are ignored.

The format of the relative time value is dependent on the date style you choose when creating the text provider. For a list of possible styles and examples of each, see CLKRelativeDateStyle.

## Topics

### Creating a Text Provider

convenience init(date: Date, style: CLKRelativeDateStyle, units: NSCalendar.Unit)

Creates a text provider that shows the difference between the current time and the specified date.

convenience init(date: Date, relativeTo: Date?, style: CLKRelativeDateStyle, units: NSCalendar.Unit)

Creates a text provider that shows the difference in time between the provided dates.

### Getting the Date Information

var date: Date

The target date to use for calculations.

var relativeToDate: Date?

The end date that the text provider uses when calculating a fixed, relative date.

var relativeDateStyle: CLKRelativeDateStyle

The formatting style to use for the relative time value.

var calendarUnits: NSCalendar.Unit

The calendar units to include in the formatted string.

### Constants

enum CLKRelativeDateStyle

Constants indicating the formatting style for the relative date values.

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

class CLKTimeIntervalTextProvider

A formatted time range.

Deprecated

class CLKTimeTextProvider

A formatted time value.

Deprecated

class CLKTextProvider

The common behavior for displaying text-based data in a complication.

Deprecated

