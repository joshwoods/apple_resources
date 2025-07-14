

- Foundation
- Calendar
-  date(bySettingHour:minute:second:of:matchingPolicy:repeatedTimePolicy:direction:) 

Instance Method

# date(bySettingHour:minute:second:of:matchingPolicy:repeatedTimePolicy:direction:)

Returns a new `Date` representing the date calculated by setting hour, minute, and second to a given time on a specified `Date`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func date(
    bySettingHour hour: Int,
    minute: Int,
    second: Int,
    of date: Date,
    matchingPolicy: Calendar.MatchingPolicy = .nextTime,
    repeatedTimePolicy: Calendar.RepeatedTimePolicy = .first,
    direction: Calendar.SearchDirection = .forward
) -> Date?
```

## Parameters 

`hour`  

A specified hour.

`minute`  

A specified minute.

`second`  

A specified second.

`date`  

The date to start calculation with.

`matchingPolicy`  

Specifies the technique the search algorithm uses to find results. Default value is `.nextTime`.

`repeatedTimePolicy`  

Specifies the behavior when multiple matches are found. Default value is `.first`.

`direction`  

Specifies the direction in time to search. Default is `.forward`.

## Return Value

A `Date` representing the result of the search, or `nil` if a result could not be found.

## Discussion

If no such time exists, the next available time is returned (which could, for example, be in a different day than the nominal target date). The intent is to return a date on the same day as the original date argument. This may result in a date which is backward than the given date, of course.

## See Also

### Calculating Dates from Components

func date(from: DateComponents) -> Date?

Returns a date created from the specified components.

func date(byAdding: DateComponents, to: Date, wrappingComponents: Bool) -> Date?

Returns a new `Date` representing the date calculated by adding components to a given date.

func date(byAdding: Calendar.Component, value: Int, to: Date, wrappingComponents: Bool) -> Date?

Returns a new `Date` representing the date calculated by adding an amount of a specific component to a given date.

func date(bySetting: Calendar.Component, value: Int, of: Date) -> Date?

Returns a new `Date` representing the date calculated by setting a specific component to a given time, and trying to keep lower components the same. If the component already has that value, this may result in a date which is the same as the given date.

