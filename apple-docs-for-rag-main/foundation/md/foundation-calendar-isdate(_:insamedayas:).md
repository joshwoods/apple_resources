

- Foundation
- Calendar
-  isDate(\_:inSameDayAs:) 

Instance Method

# isDate(\_:inSameDayAs:)

Returns a Boolean value indicating whether a date is within the same day as another date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isDate(
    _ date1: Date,
    inSameDayAs date2: Date
) -> Bool
```

## Parameters 

`date1`  

A date to check for containment.

`date2`  

A date to check for containment.

## Return Value

`true` if `date1` and `date2` are in the same day, as defined by the calendar and calendar’s locale; otherwise, `false`.

## See Also

### Comparing Dates

func compare(Date, to: Date, toGranularity: Calendar.Component) -> ComparisonResult

Compares two dates down to the specified component.

func isDate(Date, equalTo: Date, toGranularity: Calendar.Component) -> Bool

Returns a Boolean value indicating whether two dates are equal down to the specified component.

func isDateInToday(Date) -> Bool

Returns a Boolean value indicating whether the given date is within today.

func isDateInTomorrow(Date) -> Bool

Returns a Boolean value indicating whether the given date is within tomorrow.

func isDateInYesterday(Date) -> Bool

Returns a Boolean value indicating whether the given date is within yesterday.

func isDateInWeekend(Date) -> Bool

Returns a Boolean value indicating whether the given date is within a weekend period.

