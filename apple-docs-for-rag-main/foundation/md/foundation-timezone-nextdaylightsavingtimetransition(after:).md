

- Foundation
- TimeZone
-  nextDaylightSavingTimeTransition(after:) 

Instance Method

# nextDaylightSavingTimeTransition(after:)

Returns the next daylight saving time transition after a given date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func nextDaylightSavingTimeTransition(after date: Date) -> Date?
```

## Parameters 

`date`  

A date.

## Return Value

The next daylight saving time transition after `date`. Depending on the time zone, this function may return a change of the time zone’s offset from GMT. Returns `nil` if the time zone of the receiver does not observe daylight savings time as of `date`.

## See Also

### Working with Daylight Savings

func isDaylightSavingTime(for: Date) -> Bool

Returns a Boolean value that indicates whether the receiver uses daylight saving time at a given date.

func daylightSavingTimeOffset(for: Date) -> TimeInterval

Returns the daylight saving time offset for a given date.

var nextDaylightSavingTimeTransition: Date?

The date of the next (after the current instant) daylight saving time transition for the time zone.

