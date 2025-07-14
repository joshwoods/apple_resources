

- Foundation
- NSTimeZone
-  isDaylightSavingTime(for:) 

Instance Method

# isDaylightSavingTime(for:)

Indicates whether the receiver uses daylight saving time on a given date.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isDaylightSavingTime(for aDate: Date) -> Bool
```

## Parameters 

`aDate`  

The date against which to test the receiver.

## Return Value

true if the receiver uses daylight saving time at `aDate`, otherwise false.

## See Also

### Working with Daylight Savings

var isDaylightSavingTime: Bool

A Boolean value that indicates whether the receiver is currently using daylight saving time.

var daylightSavingTimeOffset: TimeInterval

The current daylight saving time offset of the receiver.

func daylightSavingTimeOffset(for: Date) -> TimeInterval

Returns the daylight saving time offset for a given date.

var nextDaylightSavingTimeTransition: Date?

The date of the next daylight saving time transition for the receiver.

func nextDaylightSavingTimeTransition(after: Date) -> Date?

Returns the next daylight saving time transition after a given date.

