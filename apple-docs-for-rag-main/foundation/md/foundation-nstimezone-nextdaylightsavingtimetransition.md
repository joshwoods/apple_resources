

- Foundation
- NSTimeZone
-  nextDaylightSavingTimeTransition 

Instance Property

# nextDaylightSavingTimeTransition

The date of the next daylight saving time transition for the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var nextDaylightSavingTimeTransition: Date? { get }
```

## Discussion

This property contains the date of the next (after the current instant) daylight saving time transition for the receiver. Depending on the time zone of the receiver, the value of this property may represent a change of the time zone’s offset from GMT. Returns `nil` if the time zone of the receiver does not currently observe daylight saving time.

## See Also

### Working with Daylight Savings

var isDaylightSavingTime: Bool

A Boolean value that indicates whether the receiver is currently using daylight saving time.

func isDaylightSavingTime(for: Date) -> Bool

Indicates whether the receiver uses daylight saving time on a given date.

var daylightSavingTimeOffset: TimeInterval

The current daylight saving time offset of the receiver.

func daylightSavingTimeOffset(for: Date) -> TimeInterval

Returns the daylight saving time offset for a given date.

func nextDaylightSavingTimeTransition(after: Date) -> Date?

Returns the next daylight saving time transition after a given date.

