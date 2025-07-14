

- Foundation
- Calendar
-  startOfDay(for:) 

Instance Method

# startOfDay(for:)

Returns the first moment of a given Date, as a Date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func startOfDay(for date: Date) -> Date
```

## Parameters 

`date`  

The date to search.

## Return Value

The first moment of the given date.

## Discussion

For example, pass in `Date()`, if you want the start of today. If there were two midnights, it returns the first. If there was none, it returns the first moment that did exist.

## See Also

### Scanning Dates

func enumerateDates(startingAfter: Date, matching: DateComponents, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, direction: Calendar.SearchDirection, using: (Date?, Bool, inout Bool) -> Void)

Computes the dates which match (or most closely match) a given set of components, and calls the closure once for each of them, until the enumeration is stopped.

func nextDate(after: Date, matching: DateComponents, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, direction: Calendar.SearchDirection) -> Date?

Computes the next date which matches (or most closely matches) a given set of components.

enum MatchingPolicy

A hint to the search algorithm to control the method used for searching for dates.

enum RepeatedTimePolicy

Determines which result to use when a time is repeated on a day in a calendar (for example, during a daylight saving transition when the times between 2:00am and 3:00am may happen twice).

