

- Foundation
- NSCalendar
-  isDateInTomorrow(\_:) 

Instance Method

# isDateInTomorrow(\_:)

Indicates whether the given date is in “tomorrow.”

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isDateInTomorrow(_ date: Date) -> Bool
```

## Parameters 

`date`  

The date for which to perform the calculation.

## Return Value

true if the given date is in “tomorrow,” otherwise false.

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

func isDateInWeekend(Date) -> Bool

Indicates whether a given date falls within a weekend period, as defined by the calendar and the calendar’s locale.

func isDateInYesterday(Date) -> Bool

Indicates whether the given date is in “yesterday.”

