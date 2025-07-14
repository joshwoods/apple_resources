

- Foundation
- Date
- Date.IntervalFormatStyle
-  month(\_:) 

Instance Method

# month(\_:)

Modifies the date interval format style to include the month.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func month(_ format: Date.IntervalFormatStyle.Symbol.Month = .abbreviated) -> Date.IntervalFormatStyle
```

## Parameters 

`format`  

The month format style to apply to the date interval format style.

## Return Value

A date interval format style that includes the specified month style.

## Discussion

Use a combination of modifier instance methods to customize the format of the date interval. The following example shows several combinations of year, month, and day components in the date interval:

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

func minute() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the minutes.

func second() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the seconds.

func weekday(Date.IntervalFormatStyle.Symbol.Weekday) -> Date.IntervalFormatStyle

Modifies the date interval format style to include the specified weekday style.

func year() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the year.

