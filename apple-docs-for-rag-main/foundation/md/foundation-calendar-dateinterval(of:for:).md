

- Foundation
- Calendar
-  dateInterval(of:for:) 

Instance Method

# dateInterval(of:for:)

Returns the starting time and duration of a given calendar component that contains a given date.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func dateInterval(
    of component: Calendar.Component,
    for date: Date
) -> DateInterval?
```

## Parameters 

`component`  

A calendar component.

`date`  

The specified date.

## Return Value

A new `DateInterval` if the starting time and duration of a component could be calculated; otherwise, `nil`.

## See Also

### Calculating Intervals

func dateInterval(of: Calendar.Component, start: inout Date, interval: inout TimeInterval, for: Date) -> Bool

Returns, via two inout parameters, the starting time and duration of a given calendar component that contains a given date.

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

