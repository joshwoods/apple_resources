

- Foundation
- Date
-  timeIntervalBetween1970AndReferenceDate 

Type Property

# timeIntervalBetween1970AndReferenceDate

The number of seconds from 1 January 1970 to the reference date, 1 January 2001.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let timeIntervalBetween1970AndReferenceDate: Double
```

## See Also

### Getting Time Intervals

func timeIntervalSince(Date) -> TimeInterval

Returns the interval between this date and another given date.

var timeIntervalSinceNow: TimeInterval

The time interval between the date value and the current date and time.

var timeIntervalSinceReferenceDate: TimeInterval

The interval between the date value and 00:00:00 UTC on 1 January 2001.

var timeIntervalSince1970: TimeInterval

The interval between the date value and 00:00:00 UTC on 1 January 1970.

static var timeIntervalSinceReferenceDate: TimeInterval

The interval between 00:00:00 UTC on 1 January 2001 and the current date and time.

