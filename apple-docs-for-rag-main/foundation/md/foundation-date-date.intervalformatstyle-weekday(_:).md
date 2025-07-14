

- Foundation
- Date
- Date.IntervalFormatStyle
-  weekday(\_:) 

Instance Method

# weekday(\_:)

Modifies the date interval format style to include the specified weekday style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func weekday(_ format: Date.IntervalFormatStyle.Symbol.Weekday = .abbreviated) -> Date.IntervalFormatStyle
```

## Parameters 

`format`  

The weekday format style to apply to the date interval format style.

## Return Value

A date interval format style that includes the specified weekday style.

## Discussion

Use a combination of modifier instance methods to customize the format of the date interval. The following example shows a combination date interval format styles that include the weekday:

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

func month(Date.IntervalFormatStyle.Symbol.Month) -> Date.IntervalFormatStyle

Modifies the date interval format style to include the month.

func second() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the seconds.

func year() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the year.

