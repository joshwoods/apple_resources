

- Foundation
- Date
- Date.FormatStyle
-  day(\_:) 

Instance Method

# day(\_:)

Modifies the date format style to use the specified day format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func day(_ format: Date.FormatStyle.Symbol.Day = .defaultDigits) -> Date.FormatStyle
```

## Parameters 

`format`  

The day format style applied to the date format style.

## Return Value

A date format style modified to include the specified day style.

## Discussion

Possible values of Date.FormatStyle.Symbol.Day are defaultDigits, ordinalOfDayInMonth, and twoDigits.

This example shows a variety of Date.FormatStyle.Symbol.Day formats applied to a date:

```
let meetingDate = Date() // Feb 9, 2021 at 3:00 PM
meetingDate.formatted(Date.FormatStyle().day(.defaultDigits)) // 9
meetingDate.formatted(Date.FormatStyle().day(.ordinalOfDayInMonth)) // 2 (second Tuesday of the month)
meetingDate.formatted(Date.FormatStyle().day(.twoDigits)) // 09
meetingDate.formatted(Date.FormatStyle().day()) // 9
```

If you don’t provide a format, the defaultDigits static variable is the default format.

For more information about formatting dates, see Date.FormatStyle.

## See Also

### Specifying the Date Format

func dayOfYear(Date.FormatStyle.Symbol.DayOfYear) -> Date.FormatStyle

Modifies the date format style to use the specified day of the year format style.

func era(Date.FormatStyle.Symbol.Era) -> Date.FormatStyle

Modifies the date format style to use the specified era format style.

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

