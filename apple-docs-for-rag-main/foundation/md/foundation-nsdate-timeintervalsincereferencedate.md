

- Foundation
- NSDate
-  timeIntervalSinceReferenceDate 

Type Property

# timeIntervalSinceReferenceDate

The interval between 00:00:00 UTC on 1 January 2001 and the current date and time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var timeIntervalSinceReferenceDate: TimeInterval { get }
```

## Return Value

The interval between the system’s absolute reference date (00:00:00 UTC on 1 January 2001) and the current date and time.

## Discussion

This method is the primitive method for NSDate. If you subclass NSDate, you must override this method with your own implementation for it.

## See Also

### Getting Time Intervals

func timeIntervalSince(Date) -> TimeInterval

Returns the interval between the receiver and another given date.

var timeIntervalSinceNow: TimeInterval

The interval between the date object and the current date and time.

var timeIntervalSinceReferenceDate: TimeInterval

The interval between the date object and 00:00:00 UTC on 1 January 2001.

var timeIntervalSince1970: TimeInterval

The interval between the date object and 00:00:00 UTC on 1 January 1970.

var NSTimeIntervalSince1970: Double

The number of seconds from 1 January 1970 to the reference date, 1 January 2001.

