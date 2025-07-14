

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.Year 

Structure

# Date.FormatStyle.Symbol.Year

A type that specifies a format for the year in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Year
```

## Overview

The Date.FormatStyle.Symbol.Year type includes static factory variables and methods that create custom Date.FormatStyle.Symbol.Year objects:

| Factory variable | Description |
|----|----|
| defaultDigits | The minimum number of digits that represents the full year. For example, `2`, `20`, `201`, `2017`. |
| twoDigits | The year’s two lowest-order digits, zero-padded or truncated if necessary. For example, `02`, `20`, `01`, `17`, `73`. |
| padded(_:) | Three or more digits, zero-padded if necessary. For example, `002`, `020`, `201`, `2017`. |
| relatedGregorian(minimumLength:) | For non-Gregorian calendars, output corresponds to the extended Gregorian year in which the calendar’s year begins. The default length is the minimum needed to show the full year. |
| extended(minimumLength:) | A single number designating the year of the calendar system, encompassing all supra-year fields. The default length is the minimum needed to show the full year. |

To customize the year format in a string representation of a `Date`, use year(_:). The following example shows a variety of Date.FormatStyle.Symbol.Year formats applied to a date.

```
let meetingDate = Date() // Feb 9, 2021 at 3:00 PM
meetingDate.formatted(Date.FormatStyle().year(.defaultDigits)) // 2021
meetingDate.formatted(Date.FormatStyle().year(.twoDigits)) // 21
meetingDate.formatted(Date.FormatStyle().year(.extended(minimumLength: 5))) // 02021
meetingDate.formatted(Date.FormatStyle().year(.extended())) // 2021
meetingDate.formatted(Date.FormatStyle().year(.padded(6))) // 002021
meetingDate.formatted(Date.FormatStyle().year(.relatedGregorian())) // 2021
```

If no format is specified as a parameter, the defaultDigits static variable is the default format.

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying a Year

static var defaultDigits: Date.FormatStyle.Symbol.Year

The custom year format style showing the minimum number of digits that represents the numeric year.

static var twoDigits: Date.FormatStyle.Symbol.Year

The custom format style portraying the two-digit numeric year, zero-padded if necessary.

static func padded(Int) -> Date.FormatStyle.Symbol.Year

Returns a custom format style that portrays the year of the calendar system of the provided length, zero-padded if necessary.

static func relatedGregorian(minimumLength: Int) -> Date.FormatStyle.Symbol.Year

Returns a custom format style that portrays the year of a non-Gregorian calendar system in the corresponding Gregorian year.

static func extended(minimumLength: Int) -> Date.FormatStyle.Symbol.Year

Returns a custom format style that portrays the year of the calendar system, encompassing all supra-year fields.

### Comparing Years

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.Year

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

