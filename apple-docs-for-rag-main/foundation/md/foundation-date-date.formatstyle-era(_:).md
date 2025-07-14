

- Foundation
- Date
- Date.FormatStyle
-  era(\_:) 

Instance Method

# era(\_:)

Modifies the date format style to use the specified era format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func era(_ format: Date.FormatStyle.Symbol.Era = .abbreviated) -> Date.FormatStyle
```

## Parameters 

`format`  

The era format style applied to the date format style.

## Return Value

A date format style modified to include the specified era style.

## Discussion

Possible values of Date.FormatStyle.Symbol.Era include abbreviated, narrow, and wide.

This example shows a variety of Date.FormatStyle.Symbol.Era format styles applied to a date:

```
let meetingDate = Date() // Feb 9, 2021 at 3:00 PM
meetingDate.formatted(Date.FormatStyle().era(.abbreviated)) // AD
meetingDate.formatted(Date.FormatStyle().era(.narrow)) // A
meetingDate.formatted(Date.FormatStyle().era(.wide)) // Anno Domini
meetingDate.formatted(Date.FormatStyle().era()) // AD
```

If you don’t provide a format, the abbreviated static variable is the default format.

For more information about formatting dates, see Date.FormatStyle.

## See Also

### Specifying the Date Format

func day(Date.FormatStyle.Symbol.Day) -> Date.FormatStyle

Modifies the date format style to use the specified day format style.

func dayOfYear(Date.FormatStyle.Symbol.DayOfYear) -> Date.FormatStyle

Modifies the date format style to use the specified day of the year format style.

func month(Date.FormatStyle.Symbol.Month) -> Date.FormatStyle

Modifies the date format style to use the specified month format style.

func quarter(Date.FormatStyle.Symbol.Quarter) -> Date.FormatStyle

Modifies the date format style to use the specified quarter format style.

func week(Date.FormatStyle.Symbol.Week) -> Date.FormatStyle

Modifies the date format style to use the specified week format style.

func weekday(Date.FormatStyle.Symbol.Weekday) -> Date.FormatStyle

Modifies the date format style to use the specified weekday format style.

func year(Date.FormatStyle.Symbol.Year) -> Date.FormatStyle

Modifies the date format style to use the specified year format style.

struct DateStyle

Type that defines date styles varied in length or components included.

