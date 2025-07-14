

- Core Foundation
-  CFTimeZoneGetDaylightSavingTimeOffset(\_:\_:) 

Function

# CFTimeZoneGetDaylightSavingTimeOffset(\_:\_:)

Returns the daylight saving time offset for a time zone at a given time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFTimeZoneGetDaylightSavingTimeOffset(
    _ tz: CFTimeZone!,
    _ at: CFAbsoluteTime
) -> CFTimeInterval
```

## Parameters 

`tz`  

The time zone to analyze.

`at`  

The time in `tz` to test for daylight saving time offset.

## Return Value

The daylight saving time offset for `tz` at `at`.

## See Also

### Getting Daylight Savings Time Information

func CFTimeZoneIsDaylightSavingTime(CFTimeZone!, CFAbsoluteTime) -> Bool

Returns whether or not a time zone is in daylight savings time at a specified date.

func CFTimeZoneGetNextDaylightSavingTimeTransition(CFTimeZone!, CFAbsoluteTime) -> CFAbsoluteTime

Returns the time in a given time zone of the next daylight saving time transition after a given time.

