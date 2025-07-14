

- EventKit
- EKEvent
-  compareStartDate(with:) 

Instance Method

# compareStartDate(with:)

Compares the start date of the receiving event with the start date of another event.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func compareStartDate(with other: EKEvent) -> ComparisonResult
```

## Parameters 

`other`  

The event to compare against.

## Return Value

Returns ComparisonResult.orderedAscending if the start date of the receiver precedes the start date of `other`. Returns ComparisonResult.orderedSame if the start dates of the two events are identical. Returns ComparisonResult.orderedDescending if the start date of the receiver comes after the start date of `other`.

## Mentioned in 

Retrieving events and reminders

## Discussion

You can pass the selector for this method to the NSArray method sortedArray(using:) to create an array of events sorted by start date.

