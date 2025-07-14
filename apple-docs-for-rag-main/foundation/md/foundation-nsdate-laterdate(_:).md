

- Foundation
- NSDate
-  laterDate(\_:) 

Instance Method

# laterDate(\_:)

Returns the later of the receiver and another given date.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func laterDate(_ anotherDate: Date) -> Date
```

## Parameters 

`anotherDate`  

The date with which to compare the receiver.

## Return Value

The later of the receiver and `anotherDate`, determined using timeIntervalSince(_:). If the receiver and `anotherDate` represent the same date, returns the receiver.

## See Also

### Related Documentation

func isEqual(_ object: Any?) -> Bool

Returns a Boolean value that indicates whether the receiver and a given object are equal.

### Comparing Dates

func isEqual(to: Date) -> Bool

Returns a Boolean value that indicates whether a given object is a date that is exactly equal the receiver.

func earlierDate(Date) -> Date

Returns the earlier of the receiver and another given date.

func compare(Date) -> ComparisonResult

Indicates the temporal ordering of the receiver and another given date.

