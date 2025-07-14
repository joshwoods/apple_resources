

- Foundation
- NSDateInterval
-  compare(\_:) 

Instance Method

# compare(\_:)

Compares the receiver with the specified date interval.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func compare(_ dateInterval: DateInterval) -> ComparisonResult
```

## Parameters 

`dateInterval`  

The date interval with which to compare the receiver.

## Return Value

Returns an ComparisonResult value that indicates the temporal ordering of the receiver and a given date interval:

- ComparisonResult.orderedAscending if the receiver’s startDate occurs earlier than that of `dateInterval`, or both startDate values are equal and the duration of the receiver is less than that of `dateInterval`.

- ComparisonResult.orderedDescending if the receiver’s startDate occurs later than that of `dateInterval`, or both startDate values are equal and the duration of the receiver is greater than that of `dateInterval`.

- ComparisonResult.orderedSame if the receiver’s startDate and duration values are equal to those of `dateInterval`.

## Discussion

The following figure illustrates four `NSDateInterval` objects plotted on an arbitrary time axis. Each date interval spans its duration from left to right, from its startDate to its endDate.

The result of comparing the date interval labeled **A** with the date interval labeled **B** is ComparisonResult.orderedAscending, because **A** has a startDate that occurs earlier than that of **B**.

The result of comparing the date interval labeled **C** with the date interval labeled **D** is ComparisonResult.orderedDescending, because because **C** and **D** have the same startDate, and **C** has a duration greater than that of **D**.

## See Also

### Comparing Date Intervals

func isEqual(to: DateInterval) -> Bool

Indicates whether the receiver is equal to the specified date interval.

