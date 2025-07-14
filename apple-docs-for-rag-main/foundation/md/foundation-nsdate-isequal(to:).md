

- Foundation
- NSDate
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Returns a Boolean value that indicates whether a given object is a date that is exactly equal the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isEqual(to otherDate: Date) -> Bool
```

## Parameters 

`otherDate`  

The date to compare with the receiver.

## Return Value

true if the `otherDate` is an NSDate object and is exactly equal to the receiver, otherwise false.

## Discussion

This method detects sub-second differences between dates. If you want to compare dates with a less fine granularity, use timeIntervalSince(_:) to compare the two dates.

## See Also

### Related Documentation

func isEqual(_ object: Any?) -> Bool

Returns a Boolean value that indicates whether the receiver and a given object are equal.

### Comparing Dates

func earlierDate(Date) -> Date

Returns the earlier of the receiver and another given date.

func laterDate(Date) -> Date

Returns the later of the receiver and another given date.

func compare(Date) -> ComparisonResult

Indicates the temporal ordering of the receiver and another given date.

