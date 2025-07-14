

- Foundation
- Date
- Date.IntervalFormatStyle
-  minute() 

Instance Method

# minute()

Modifies the date interval format style to include the minutes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func minute() -> Date.IntervalFormatStyle
```

## Return Value

A date interval format style that includes the minutes.

## Discussion

This example shows a combination of date interval format styles that includes the hour and minutes:

```
if let today = Calendar.current.date(byAdding: .day, value: -140, to: Date()),
   let sevenDaysBeforeToday = Calendar.current.date(byAdding: .day, value: -7, to: today) {

    // Create a Range.
    let weekBefore = sevenDaysBeforeToday..

## See Also

### Modifying Date Interval Format Styles

func day() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the day.

func hour(Date.IntervalFormatStyle.Symbol.Hour) -> Date.IntervalFormatStyle

Modifies the date interval format style to use the specified hour format style.

func month(Date.IntervalFormatStyle.Symbol.Month) -> Date.IntervalFormatStyle

Modifies the date interval format style to include the month.

func second() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the seconds.

func weekday(Date.IntervalFormatStyle.Symbol.Weekday) -> Date.IntervalFormatStyle

Modifies the date interval format style to include the specified weekday style.

func year() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the year.

