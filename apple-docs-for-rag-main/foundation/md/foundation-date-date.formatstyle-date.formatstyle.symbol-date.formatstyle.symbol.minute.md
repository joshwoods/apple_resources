

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.Minute 

Structure

# Date.FormatStyle.Symbol.Minute

A type that specifies the format for the minutes in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Minute
```

## Overview

The type Date.FormatStyle.Symbol.Minute includes static factory variables that create custom Date.FormatStyle.Symbol.Minute objects:

| Factory variable | Description |
|----|----|
| defaultDigits | The minimum number of digits that represents the numeric minute. For example, `1`, `18`. |
| twoDigits | Two-digit numeric minute, zero-padded if necessary. For example, `01`, `18`. |

To customize the minute format in a string representation of a `Date`, use minute(_:). The following example shows a variety of Date.FormatStyle.Symbol.Minute format styles applied to a date.

```
let meetingDate = Date() // Feb 9, 2021 at 3:05 PM
meetingDate.formatted(Date.FormatStyle().minute(.defaultDigits)) // 5
meetingDate.formatted(Date.FormatStyle().minute(.twoDigits)) // 05
meetingDate.formatted(Date.FormatStyle().minute()) // 5
```

If no format is specified as a parameter, the defaultDigits static variable is the default format.

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying a Minute

static var defaultDigits: Date.FormatStyle.Symbol.Minute

The custom minute format style showing the minimum number of digits that represents the numeric minute.

static var twoDigits: Date.FormatStyle.Symbol.Minute

The custom format style that shows the two-digit numeric minute, zero-padded if necessary.

### Comparing a Minute

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.Minute

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Modifying Date Style Format Symbols

struct CyclicYear

A type that specifies a format for a cyclic year in a date format style.

struct Day

A type that specifies the format for a day in a date format style.

struct DayOfYear

A type that specifies the format for the day of the year in a date format style.

struct DayPeriod

A type that specifies a format for the time period in a date format style.

struct Era

A type that specifies a format for the era in a date format style.

struct Hour

A type that specifies a format for the hour in a date format style.

struct Month

A type that specifies a format for the month in a date format style.

struct Quarter

A type that specifies the format for the quarter in a date format style.

struct Second

A type that specifies the format for the seconds in a date format style.

struct SecondFraction

A type that specifies the format for the second fraction in a date format style.

struct StandaloneMonth

A type that specifies the format for a standalone month.

struct StandaloneQuarter

A type that specifies the format for a standalone quarter.

struct StandaloneWeekday

A type that specifies the format for a standalone weekday.

struct TimeZone

A type that specifies a format for the time zone in a date format style.

struct VerbatimHour

A type that specifies a format for the hour in a date format style.

