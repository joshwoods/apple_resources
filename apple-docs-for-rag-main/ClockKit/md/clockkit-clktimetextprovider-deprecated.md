

- ClockKit
-  CLKTimeTextProvider Deprecated

Class

# CLKTimeTextProvider

A formatted time value.

watchOS 2.0–9.0Deprecated

``` source
class CLKTimeTextProvider
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Creating a timeline entry

## Overview

This provider supports time values in either the 24-hour or 12-hour format and takes into account the user’s region and locale settings. As needed, the provider automatically shortens the string to fit the available space.

When formatting the time, the time text provider drops the morning/evening indicator if it can’t fit the entire time value. For example, a provider configured to display the time 10:09AM in the English-US locale would remove elements as follows until it encountered a string that fit the available space:

- `10:09AM`

- `10:09`

## Topics

### Creating a Text Provider

convenience init(date: Date)

Creates and returns a text provider for displaying the specified time.

convenience init(date: Date, timeZone: TimeZone?)

Creates and returns a text provider for displaying the specified time.

### Getting the Time Information

var date: Date

The date object containing the time value.

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

class CLKTimeIntervalTextProvider

A formatted time range.

Deprecated

class CLKTextProvider

The common behavior for displaying text-based data in a complication.

Deprecated

