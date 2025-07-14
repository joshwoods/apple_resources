

- Foundation
- NSCalendar
-  isDateInWeekend(\_:) 

Instance Method

# isDateInWeekend(\_:)

Indicates whether a given date falls within a weekend period, as defined by the calendar and the calendar’s locale.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isDateInWeekend(_ date: Date) -> Bool
```

## Parameters 

`date`  

The date for which to perform the calculation.

## Return Value

true if the given date is within a weekend period, otherwise false.

## Discussion

If the date does fall within a weekend, you can use the range(ofWeekendStart:interval:containing:) method to determine the start date of that weekend period. Otherwise, you can use the nextWeekendStart(_:interval:options:after:) method to determine the start date of the next or previous weekend.

## See Also

### Comparing Dates

func compare(Date, to: Date, toUnitGranularity: NSCalendar.Unit) -> ComparisonResult

Indicates the ordering of two given dates based on their components down to a given unit granularity.

func isDate(Date, equalTo: Date, toUnitGranularity: NSCalendar.Unit) -> Bool

Indicates whether two dates are equal to a given unit of granularity.

func isDate(Date, inSameDayAs: Date) -> Bool

Indicates whether two dates are in the same day.

func isDateInToday(Date) -> Bool

Indicates whether the given date is in “today.”

func isDateInTomorrow(Date) -> Bool

Indicates whether the given date is in “tomorrow.”

func isDateInYesterday(Date) -> Bool

Indicates whether the given date is in “yesterday.”

