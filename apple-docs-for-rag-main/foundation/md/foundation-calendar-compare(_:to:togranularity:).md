

- Foundation
- Calendar
-  compare(\_:to:toGranularity:) 

Instance Method

# compare(\_:to:toGranularity:)

Compares two dates down to the specified component.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func compare(
    _ date1: Date,
    to date2: Date,
    toGranularity component: Calendar.Component
) -> ComparisonResult
```

## Parameters 

`date1`  

A date to compare.

`date2`  

A date to compare.

`component`  

A granularity to compare. For example, pass `.hour` to check if two dates are in the same hour.

## Return Value

`.orderedSame` if the two dates are equal in the given component and all larger components; otherwise, either `.orderedAscending` or `.orderedDescending`.

## See Also

### Comparing Dates

func isDate(Date, equalTo: Date, toGranularity: Calendar.Component) -> Bool

Returns a Boolean value indicating whether two dates are equal down to the specified component.

func isDate(Date, inSameDayAs: Date) -> Bool

Returns a Boolean value indicating whether a date is within the same day as another date.

func isDateInToday(Date) -> Bool

Returns a Boolean value indicating whether the given date is within today.

func isDateInTomorrow(Date) -> Bool

Returns a Boolean value indicating whether the given date is within tomorrow.

func isDateInYesterday(Date) -> Bool

Returns a Boolean value indicating whether the given date is within yesterday.

func isDateInWeekend(Date) -> Bool

Returns a Boolean value indicating whether the given date is within a weekend period.

