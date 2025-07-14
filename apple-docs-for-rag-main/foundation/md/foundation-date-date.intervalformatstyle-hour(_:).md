

- Foundation
- Date
- Date.IntervalFormatStyle
-  hour(\_:) 

Instance Method

# hour(\_:)

Modifies the date interval format style to use the specified hour format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func hour(_ format: Date.IntervalFormatStyle.Symbol.Hour = .defaultDigits(amPM: .abbreviated)) -> Date.IntervalFormatStyle
```

## Parameters 

`format`  

The hour format style to apply to the date interval format style.

## Return Value

A date interval format style that includes the specified hour style.

## Discussion

The values of `Date.FormatStyle.Symbol.Hour` are `defaultDigitsNoAMPM` and `twoDigitsNoAMPM`.

The static methods that return Date.FormatStyle.Symbol.Hour objectsinclude````  ```Date/FormatStyle/Symbol/Hour/conversationalDefaultDigits(amPM:)```, ```` \`\`Date/FormatStyle/Symbol/Hour/conversationalTwoDigits(amPM:)`` ,` and`  ``Date/FormatStyle/Symbol/Hour/defaultDigits(amPM:)\`\`\`.\`

This example shows a variety of Date.FormatStyle.Symbol.Hour format styles for a date interval:

```
if let today = Calendar.current.date(byAdding: .day, value: -140, to: Date()),
   let sevenDaysBeforeToday = Calendar.current.date(byAdding: .day, value: -7, to: today) {

    // Create a Range.
    let weekBefore = sevenDaysBeforeToday..

## See Also

### Modifying Date Interval Format Styles

func day() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the day.

func minute() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the minutes.

func month(Date.IntervalFormatStyle.Symbol.Month) -> Date.IntervalFormatStyle

Modifies the date interval format style to include the month.

func second() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the seconds.

func weekday(Date.IntervalFormatStyle.Symbol.Weekday) -> Date.IntervalFormatStyle

Modifies the date interval format style to include the specified weekday style.

func year() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the year.

