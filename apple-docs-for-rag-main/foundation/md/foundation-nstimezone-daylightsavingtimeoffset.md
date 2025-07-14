

- Foundation
- NSTimeZone
-  daylightSavingTimeOffset 

Instance Property

# daylightSavingTimeOffset

The current daylight saving time offset of the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var daylightSavingTimeOffset: TimeInterval { get }
```

## See Also

### Working with Daylight Savings

var isDaylightSavingTime: Bool

A Boolean value that indicates whether the receiver is currently using daylight saving time.

func isDaylightSavingTime(for: Date) -> Bool

Indicates whether the receiver uses daylight saving time on a given date.

func daylightSavingTimeOffset(for: Date) -> TimeInterval

Returns the daylight saving time offset for a given date.

var nextDaylightSavingTimeTransition: Date?

The date of the next daylight saving time transition for the receiver.

func nextDaylightSavingTimeTransition(after: Date) -> Date?

Returns the next daylight saving time transition after a given date.

