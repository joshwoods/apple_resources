

- Foundation
- Date
- Date.FormatStyle
-  weekday(\_:) 

Instance Method

# weekday(\_:)

Modifies the date format style to use the specified weekday format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func weekday(_ format: Date.FormatStyle.Symbol.Weekday = .abbreviated) -> Date.FormatStyle
```

## Parameters 

`format`  

The weekday format style applied to the date format style.

## Return Value

A date format style modified to include the specified week format style.

## Discussion

Possible values of Date.FormatStyle.Symbol.Weekday include abbreviated, narrow, oneDigit, short, twoDigits, and wide.

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

func year(Date.FormatStyle.Symbol.Year) -> Date.FormatStyle

Modifies the date format style to use the specified year format style.

struct DateStyle

Type that defines date styles varied in length or components included.

