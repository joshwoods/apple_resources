

- Foundation
- Calendar
-  dateInterval(of:start:interval:for:) 

Instance Method

# dateInterval(of:start:interval:for:)

Returns, via two inout parameters, the starting time and duration of a given calendar component that contains a given date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dateInterval(
    of component: Calendar.Component,
    start: inout Date,
    interval: inout TimeInterval,
    for date: Date
) -> Bool
```

## Parameters 

`component`  

A calendar component.

`start`  

Upon return, the starting time of the calendar component that contains the date.

`interval`  

Upon return, the duration of the calendar component that contains the date.

`date`  

The specified date.

## Return Value

`true` if the starting time and duration of a component could be calculated; otherwise, `false`.

## See Also

### Calculating Intervals

func dateInterval(of: Calendar.Component, for: Date) -> DateInterval?

Returns the starting time and duration of a given calendar component that contains a given date.

func dateIntervalOfWeekend(containing: Date) -> DateInterval?

Returns a `DateInterval` of the weekend contained by the given date, or `nil` if the date is not in a weekend.

func dateIntervalOfWeekend(containing: Date, start: inout Date, interval: inout TimeInterval) -> Bool

Find the range of the weekend around the given date, returned via two by-reference parameters.

func nextWeekend(startingAfter: Date, direction: Calendar.SearchDirection) -> DateInterval?

Returns a `DateInterval` of the next weekend, which starts strictly after the given date.

func nextWeekend(startingAfter: Date, start: inout Date, interval: inout TimeInterval, direction: Calendar.SearchDirection) -> Bool

Returns the range of the next weekend via two inout parameters. The weekend starts strictly after the given date.

enum SearchDirection

The direction in time to search.

