

- Foundation
- NSCalendar
-  isDate(\_:inSameDayAs:) 

Instance Method

# isDate(\_:inSameDayAs:)

Indicates whether two dates are in the same day.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isDate(
    _ date1: Date,
    inSameDayAs date2: Date
) -> Bool
```

## Parameters 

`date1`  

The first date to compare.

`date2`  

The second date to compare.

## Return Value

true if both dates are within the same day, otherwise false.

## See Also

### Comparing Dates

func compare(Date, to: Date, toUnitGranularity: NSCalendar.Unit) -> ComparisonResult

Indicates the ordering of two given dates based on their components down to a given unit granularity.

func isDate(Date, equalTo: Date, toUnitGranularity: NSCalendar.Unit) -> Bool

Indicates whether two dates are equal to a given unit of granularity.

func isDateInToday(Date) -> Bool

Indicates whether the given date is in “today.”

func isDateInTomorrow(Date) -> Bool

Indicates whether the given date is in “tomorrow.”

func isDateInWeekend(Date) -> Bool

Indicates whether a given date falls within a weekend period, as defined by the calendar and the calendar’s locale.

func isDateInYesterday(Date) -> Bool

Indicates whether the given date is in “yesterday.”

