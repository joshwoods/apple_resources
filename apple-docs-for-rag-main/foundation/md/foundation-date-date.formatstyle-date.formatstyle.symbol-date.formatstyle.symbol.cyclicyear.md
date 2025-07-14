

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.CyclicYear 

Structure

# Date.FormatStyle.Symbol.CyclicYear

A type that specifies a format for a cyclic year in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct CyclicYear
```

## Overview

Calendars such as the Chinese lunar calendar and Hindu calendars use 60-year cycles of year names. If the calendar doesn’t provide cyclic year-name data, or if the year value to format is out of the range of years for which the system provides cyclic name data, then the formatting is numeric, as in Date.FormatStyle.Symbol.Year.

The Date.FormatStyle.Symbol.CyclicYear type includes static factory variables that create custom Date.FormatStyle.Symbol.CyclicYear objects:

| Factory variable | Description |
|----|----|
| abbreviated | A shortened representation of the cyclic year appropriate for space-constrained applications. |
| narrow | The shortest representation of the cyclic year. |
| wide | The full representation of the cyclic year. |

If no format is specified as a parameter, the abbreviated static variable is the default format.

For more information about formatting dates, see Date.FormatStyle.

## Topics

### Modifying a Cyclic Year

static var abbreviated: Date.FormatStyle.Symbol.CyclicYear

Custom cyclic year format style that portrays a shortened cyclic year.

static var narrow: Date.FormatStyle.Symbol.CyclicYear

Custom cyclic year format style that portrays the shortest representation of a cyclic year.

static var wide: Date.FormatStyle.Symbol.CyclicYear

Custom cyclic year format style that portrays a complete representation of a cyclic year.

### Comparing Cyclic Years

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.CyclicYear

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Modifying Date Style Format Symbols

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

