

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.Era 

Structure

# Date.FormatStyle.Symbol.Era

A type that specifies a format for the era in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Era
```

## Overview

The type Date.FormatStyle.Symbol.Era includes static factory variables that create custom Date.FormatStyle.Symbol.Era objects.

| Factory variable | Description |
|----|----|
| abbreviated | An abbreviated representation of an era. For example, `AD`, `BC`. |
| narrow | A narrow era representation. For example, `A`, `B`. |
| wide | A full representation of an era. For example, `Anno Domini`, `Before Christ`. |

To customize the era format in a string representation of a `Date`, use era(_:). The following example shows a variety of Date.FormatStyle.Symbol.Era format styles applied to a date.

```
let meetingDate = Date() // Feb 9, 2021 at 3:00 PM
meetingDate.formatted(Date.FormatStyle().era(.abbreviated)) // AD
meetingDate.formatted(Date.FormatStyle().era(.narrow)) // A
meetingDate.formatted(Date.FormatStyle().era(.wide)) // Anno Domini
meetingDate.formatted(Date.FormatStyle().era()) // AD
```

If no format is specified as a parameter, the abbreviated static variable is the default format.

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying an Era

static var abbreviated: Date.FormatStyle.Symbol.Era

An abbreviated representation of an era.

static var narrow: Date.FormatStyle.Symbol.Era

A narrow representation of an era.

static var wide: Date.FormatStyle.Symbol.Era

A full representation of an era.

### Comparing an Era

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.Era

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

struct Hour

A type that specifies a format for the hour in a date format style.

struct Minute

A type that specifies the format for the minutes in a date format style.

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

