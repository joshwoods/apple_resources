

- Foundation
- Calendar
-  isDateInYesterday(\_:) 

Instance Method

# isDateInYesterday(\_:)

Returns a Boolean value indicating whether the given date is within yesterday.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isDateInYesterday(_ date: Date) -> Bool
```

## Parameters 

`date`  

The specified date.

## Return Value

`true` if the given date is within yesterday, as defined by the calendar and calendar’s locale; otherwise, `false`.

## See Also

### Comparing Dates

func compare(Date, to: Date, toGranularity: Calendar.Component) -> ComparisonResult

Compares two dates down to the specified component.

func isDate(Date, equalTo: Date, toGranularity: Calendar.Component) -> Bool

Returns a Boolean value indicating whether two dates are equal down to the specified component.

func isDate(Date, inSameDayAs: Date) -> Bool

Returns a Boolean value indicating whether a date is within the same day as another date.

func isDateInToday(Date) -> Bool

Returns a Boolean value indicating whether the given date is within today.

func isDateInTomorrow(Date) -> Bool

Returns a Boolean value indicating whether the given date is within tomorrow.

func isDateInWeekend(Date) -> Bool

Returns a Boolean value indicating whether the given date is within a weekend period.

