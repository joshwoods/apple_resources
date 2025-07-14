

- Foundation
- Date
-  timeIntervalSince(\_:) 

Instance Method

# timeIntervalSince(\_:)

Returns the interval between this date and another given date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func timeIntervalSince(_ date: Date) -> TimeInterval
```

## Parameters 

`date`  

The date with which to compare this one.

## Return Value

The interval between the receiver and the `another` parameter. If the receiver is earlier than `anotherDate`, the return value is negative. If `anotherDate` is `nil`, the results are undefined.

## See Also

### Getting Time Intervals

var timeIntervalSinceNow: TimeInterval

The time interval between the date value and the current date and time.

var timeIntervalSinceReferenceDate: TimeInterval

The interval between the date value and 00:00:00 UTC on 1 January 2001.

var timeIntervalSince1970: TimeInterval

The interval between the date value and 00:00:00 UTC on 1 January 1970.

static var timeIntervalSinceReferenceDate: TimeInterval

The interval between 00:00:00 UTC on 1 January 2001 and the current date and time.

static let timeIntervalBetween1970AndReferenceDate: Double

The number of seconds from 1 January 1970 to the reference date, 1 January 2001.

