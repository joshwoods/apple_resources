

- Foundation
- NSDate
-  compare(\_:) 

Instance Method

# compare(\_:)

Indicates the temporal ordering of the receiver and another given date.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func compare(_ other: Date) -> ComparisonResult
```

## Parameters 

`other`  

The date with which to compare the receiver.

This value must not be `nil`. If the value is `nil`, the behavior is undefined and may change in future versions of macOS.

## Return Value

If:

- The receiver and `anotherDate` are exactly equal to each other, ComparisonResult.orderedSame

- The receiver is later in time than `anotherDate`, ComparisonResult.orderedDescending

- The receiver is earlier in time than `anotherDate`, ComparisonResult.orderedAscending.

## Discussion

This method detects sub-second differences between dates. If you want to compare dates with a less fine granularity, use timeIntervalSince(_:) to compare the two dates.

## See Also

### Related Documentation

func isEqual(_ object: Any?) -> Bool

Returns a Boolean value that indicates whether the receiver and a given object are equal.

### Comparing Dates

func isEqual(to: Date) -> Bool

Returns a Boolean value that indicates whether a given object is a date that is exactly equal the receiver.

func earlierDate(Date) -> Date

Returns the earlier of the receiver and another given date.

func laterDate(Date) -> Date

Returns the later of the receiver and another given date.

