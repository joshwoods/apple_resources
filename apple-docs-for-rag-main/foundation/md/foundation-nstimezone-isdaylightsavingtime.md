

- Foundation
- NSTimeZone
-  isDaylightSavingTime 

Instance Property

# isDaylightSavingTime

A Boolean value that indicates whether the receiver is currently using daylight saving time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isDaylightSavingTime: Bool { get }
```

## Discussion

If true, the receiver is currently using daylight saving time, otherwise false. This property invokes isDaylightSavingTime(for:) with the current date as the argument.

## See Also

### Working with Daylight Savings

func isDaylightSavingTime(for: Date) -> Bool

Indicates whether the receiver uses daylight saving time on a given date.

var daylightSavingTimeOffset: TimeInterval

The current daylight saving time offset of the receiver.

func daylightSavingTimeOffset(for: Date) -> TimeInterval

Returns the daylight saving time offset for a given date.

var nextDaylightSavingTimeTransition: Date?

The date of the next daylight saving time transition for the receiver.

func nextDaylightSavingTimeTransition(after: Date) -> Date?

Returns the next daylight saving time transition after a given date.

