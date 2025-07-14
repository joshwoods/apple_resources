

- Foundation
- Calendar
-  dateIntervalOfWeekend(containing:start:interval:) 

Instance Method

# dateIntervalOfWeekend(containing:start:interval:)

Find the range of the weekend around the given date, returned via two by-reference parameters.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dateIntervalOfWeekend(
    containing date: Date,
    start: inout Date,
    interval: inout TimeInterval
) -> Bool
```

## Parameters 

`date`  

The date at which to start the search.

`start`  

When the result is `true`, set

## Return Value

`true` if a date range could be found, and `false` if the date is not in a weekend.

## Discussion

Note that a given entire day within a calendar is not necessarily all in a weekend or not; weekends can start in the middle of a day in some calendars and locales.

## See Also

### Calculating Intervals

func dateInterval(of: Calendar.Component, for: Date) -> DateInterval?

Returns the starting time and duration of a given calendar component that contains a given date.

func dateInterval(of: Calendar.Component, start: inout Date, interval: inout TimeInterval, for: Date) -> Bool

Returns, via two inout parameters, the starting time and duration of a given calendar component that contains a given date.

func dateIntervalOfWeekend(containing: Date) -> DateInterval?

Returns a `DateInterval` of the weekend contained by the given date, or `nil` if the date is not in a weekend.

func nextWeekend(startingAfter: Date, direction: Calendar.SearchDirection) -> DateInterval?

Returns a `DateInterval` of the next weekend, which starts strictly after the given date.

func nextWeekend(startingAfter: Date, start: inout Date, interval: inout TimeInterval, direction: Calendar.SearchDirection) -> Bool

Returns the range of the next weekend via two inout parameters. The weekend starts strictly after the given date.

enum SearchDirection

The direction in time to search.

