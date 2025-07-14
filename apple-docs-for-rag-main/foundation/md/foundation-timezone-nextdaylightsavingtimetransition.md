

- Foundation
- TimeZone
-  nextDaylightSavingTimeTransition 

Instance Property

# nextDaylightSavingTimeTransition

The date of the next (after the current instant) daylight saving time transition for the time zone.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var nextDaylightSavingTimeTransition: Date? { get }
```

## Discussion

Depending on the time zone, the value of this property may represent a change of the time zone’s offset from GMT. The value is `nil` if the time zone does not currently observe daylight saving time.

## See Also

### Working with Daylight Savings

func isDaylightSavingTime(for: Date) -> Bool

Returns a Boolean value that indicates whether the receiver uses daylight saving time at a given date.

func daylightSavingTimeOffset(for: Date) -> TimeInterval

Returns the daylight saving time offset for a given date.

func nextDaylightSavingTimeTransition(after: Date) -> Date?

Returns the next daylight saving time transition after a given date.

