

- Foundation
- Date
-  timeIntervalSince1970 

Instance Property

# timeIntervalSince1970

The interval between the date value and 00:00:00 UTC on 1 January 1970.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var timeIntervalSince1970: TimeInterval { get }
```

## Discussion

This property’s value is negative if the date object is earlier than 00:00:00 UTC on 1 January 1970.

## See Also

### Getting Time Intervals

func timeIntervalSince(Date) -> TimeInterval

Returns the interval between this date and another given date.

var timeIntervalSinceNow: TimeInterval

The time interval between the date value and the current date and time.

var timeIntervalSinceReferenceDate: TimeInterval

The interval between the date value and 00:00:00 UTC on 1 January 2001.

static var timeIntervalSinceReferenceDate: TimeInterval

The interval between 00:00:00 UTC on 1 January 2001 and the current date and time.

static let timeIntervalBetween1970AndReferenceDate: Double

The number of seconds from 1 January 1970 to the reference date, 1 January 2001.

