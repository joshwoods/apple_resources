

- Foundation
- Calendar
-  Calendar.RepeatedTimePolicy 

Enumeration

# Calendar.RepeatedTimePolicy

Determines which result to use when a time is repeated on a day in a calendar (for example, during a daylight saving transition when the times between 2:00am and 3:00am may happen twice).

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum RepeatedTimePolicy
```

## Topics

### Enumeration Cases

case first

If there are two or more matching times (all the components are the same, including isLeapMonth) before the end of the next instance of the next higher component to the highest specified component, then the algorithm will return the first occurrence.

case last

If there are two or more matching times (all the components are the same, including isLeapMonth) before the end of the next instance of the next higher component to the highest specified component, then the algorithm will return the last occurrence.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Scanning Dates

func startOfDay(for: Date) -> Date

Returns the first moment of a given Date, as a Date.

func enumerateDates(startingAfter: Date, matching: DateComponents, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, direction: Calendar.SearchDirection, using: (Date?, Bool, inout Bool) -> Void)

Computes the dates which match (or most closely match) a given set of components, and calls the closure once for each of them, until the enumeration is stopped.

func nextDate(after: Date, matching: DateComponents, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, direction: Calendar.SearchDirection) -> Date?

Computes the next date which matches (or most closely matches) a given set of components.

enum MatchingPolicy

A hint to the search algorithm to control the method used for searching for dates.

