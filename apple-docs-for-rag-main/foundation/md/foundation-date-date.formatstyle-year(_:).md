

- Foundation
- Date
- Date.FormatStyle
-  year(\_:) 

Instance Method

# year(\_:)

Modifies the date format style to use the specified year format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func year(_ format: Date.FormatStyle.Symbol.Year = .defaultDigits) -> Date.FormatStyle
```

## Parameters 

`format`  

The year format style applied to the date format style.

## Return Value

A date format style modified to include the specified year format style.

## Discussion

Possible values of Date.FormatStyle.Symbol.Year include twoDigits, padded(_:), relatedGregorian(minimumLength:), and extended(minimumLength:).

This example shows a variety of Date.FormatStyle.Symbol.Year formats applied to a date:

```
let meetingDate = Date() // Feb 9, 2021 at 3:00 PM
meetingDate.formatted(Date.FormatStyle().year(.defaultDigits)) // 2021
meetingDate.formatted(Date.FormatStyle().year(.twoDigits)) // 21
meetingDate.formatted(Date.FormatStyle().year(.padded(6))) // 002021
```

If you don’t provide a format, the defaultDigits static variable is the default format.

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

func week(Date.FormatStyle.Symbol.Week) -> Date.FormatStyle

Modifies the date format style to use the specified week format style.

func weekday(Date.FormatStyle.Symbol.Weekday) -> Date.FormatStyle

Modifies the date format style to use the specified weekday format style.

struct DateStyle

Type that defines date styles varied in length or components included.

