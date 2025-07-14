

- Foundation
- Date
- Date.FormatStyle
-  week(\_:) 

Instance Method

# week(\_:)

Modifies the date format style to use the specified week format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func week(_ format: Date.FormatStyle.Symbol.Week = .defaultDigits) -> Date.FormatStyle
```

## Parameters 

`format`  

The week format style applied to the date format style.

## Return Value

A date format style modified to include the specified week format style.

## Discussion

Possible values of Date.FormatStyle.Symbol.Week include defaultDigits, twoDigits, and weekOfMonth.

This example shows a variety of Date.FormatStyle.Symbol.Week format styles applied to a date:

```
let meetingDate = Date() // May 3, 2021 at 3:00 PM
meetingDate.formatted(Date.FormatStyle().week(.defaultDigits)) // 19
meetingDate.formatted(Date.FormatStyle().week(.twoDigits)) // 19
meetingDate.formatted(Date.FormatStyle().week(.weekOfMonth)) // 2
meetingDate.formatted(Date.FormatStyle().week()) // 19

```

An incomplete week at the start of a month is the first week of the month `1`. If you don’t provide a format, the defaultDigits static variable is the default format.

For more information about formatting dates, see Date.FormatStyle.

## See Also

### Specifying the Date Format

func day(Date.FormatStyle.Symbol.Day) -> Date.FormatStyle

Modifies the date format style to use the specified day format style.

func dayOfYear(Date.FormatStyle.Symbol.DayOfYear) -> Date.FormatStyle

Modifies the date format style to use the specified day of the year format style.

func era(Date.FormatStyle.Symbol.Era) -> Date.FormatStyle

Modifies the date format style to use the specified era format style.

func month(Date.FormatStyle.Symbol.Month) -> Date.FormatStyle

Modifies the date format style to use the specified month format style.

func quarter(Date.FormatStyle.Symbol.Quarter) -> Date.FormatStyle

Modifies the date format style to use the specified quarter format style.

func weekday(Date.FormatStyle.Symbol.Weekday) -> Date.FormatStyle

Modifies the date format style to use the specified weekday format style.

func year(Date.FormatStyle.Symbol.Year) -> Date.FormatStyle

Modifies the date format style to use the specified year format style.

struct DateStyle

Type that defines date styles varied in length or components included.

