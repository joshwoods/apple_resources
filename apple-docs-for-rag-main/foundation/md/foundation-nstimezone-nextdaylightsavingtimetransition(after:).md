

- Foundation
- NSTimeZone
-  nextDaylightSavingTimeTransition(after:) 

Instance Method

# nextDaylightSavingTimeTransition(after:)

Returns the next daylight saving time transition after a given date.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func nextDaylightSavingTimeTransition(after aDate: Date) -> Date?
```

## Parameters 

`aDate`  

A date.

## Return Value

The next daylight saving time transition after `aDate`. Depending on the time zone of the receiver, this method may return a change of the time zone’s offset from GMT. Returns `nil` if the time zone of the receiver does not observe daylight savings time as of `aDate`.

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

var nextDaylightSavingTimeTransition: Date?

The date of the next daylight saving time transition for the receiver.

