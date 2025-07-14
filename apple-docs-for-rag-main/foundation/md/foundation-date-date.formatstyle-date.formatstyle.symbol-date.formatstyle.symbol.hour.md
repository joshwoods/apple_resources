

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.Hour 

Structure

# Date.FormatStyle.Symbol.Hour

A type that specifies a format for the hour in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Hour
```

## Overview

The type Date.FormatStyle.Symbol.Hour includes static factory variables and methods that create custom Date.FormatStyle.Symbol.Hour objects:

| Factory variable | Description |
|----|----|
| defaultDigitsNoAMPM | The minimum number of digits that represents the full numeric hour. This doesn’t include the day period (a.m. or p.m.). For example, `1`, `11`. |
| twoDigitsNoAMPM | Two-digit numeric hour, zero-padded if necessary. This doesn’t include the day period (a.m. or p.m.). For example, `01`, `11`. |
| defaultDigits(amPM:) | The minimum number of digits that represents the full numeric hour. This may include the day period (a.m. or p.m.), depending on locale. For example, `7a` (`narrow`), `7AM` (`abbreviated`), `7A.M.` (`wide`). |
| twoDigits(amPM:) | Two-digit numeric hour, zero-padded if necessary. This may include the day period (a.m. or p.m.), depending on locale. For example, `07a` (`narrow`), `07AM` (`abbreviated`), `07A.M.` (`wide`). |
| conversationalDefaultDigits(amPM:) | The minimum number of digits that represents the full numeric hour. This may include the day period (a.m. or p.m.), depending on locale, and can include conversational period formats. For example, `7a` (`narrow`), `7AM` (`abbreviated`), `7A.M.` (`wide`). |
| conversationalTwoDigits(amPM:) | Two-digit numeric hour, zero-padded if necessary. This may include the day period (a.m. or p.m.), depending on locale, and can include conversational period formats. For example, `07a` (`narrow`), `07AM` (`abbreviated`), `07A.M.` (`wide`). |

To customize the hour format in a string representation of a `Date`, use hour(_:) The example below shows a variety of Date.FormatStyle.Symbol.Hour format styles applied to a date.

```
let meetingDate = Date() // Feb 9, 2021 at 7:00 PM
meetingDate.formatted(Date.FormatStyle().hour(.defaultDigitsNoAMPM)) 
// 7

meetingDate.formatted(Date.FormatStyle().hour(.twoDigitsNoAMPM)) 
// 07

meetingDate.formatted(Date.FormatStyle().hour(.defaultDigits(amPM: .narrow))) 
// 7p

meetingDate.formatted(Date.FormatStyle().hour(.twoDigits(amPM: .abbreviated))
// 07 PM

meetingDate.formatted(Date.FormatStyle().hour(.conversationalDefaultDigits(amPM: .wide))
// 7 P.M.
```

If no format is specified as a parameter, the defaultDigits static variable is the default format.

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying an Hour

static var defaultDigitsNoAMPM: Date.FormatStyle.Symbol.Hour

Custom format style portraying the minimum number of digits that represents the numeric hour.

Deprecated

static var twoDigitsNoAMPM: Date.FormatStyle.Symbol.Hour

Custom format style portraying the numeric hour using two digits.

Deprecated

static func conversationalDefaultDigits(amPM: Date.FormatStyle.Symbol.Hour.AMPMStyle) -> Date.FormatStyle.Symbol.Hour

Custom format style portraying the minimum number of digits that represents the hour and locale-dependent conversational day period formats.

static func conversationalTwoDigits(amPM: Date.FormatStyle.Symbol.Hour.AMPMStyle) -> Date.FormatStyle.Symbol.Hour

Custom format style portraying two digits that represent the hour and locale-dependent conversational day period formats.

static func defaultDigits(amPM: Date.FormatStyle.Symbol.Hour.AMPMStyle) -> Date.FormatStyle.Symbol.Hour

Custom format style portraying the minimum number of digits that represents the hour and locale-dependent day period formats.

static func twoDigits(amPM: Date.FormatStyle.Symbol.Hour.AMPMStyle) -> Date.FormatStyle.Symbol.Hour

Custom format style portraying two digits that represent the hour and locale-dependent day period formats.

### Supporting Structures

struct AMPMStyle

The format style of the string representation of the day period, before or after noon, in a date.

### Comparing an Hour

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.Hour

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

