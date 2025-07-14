

- Core Foundation
-  CFTimeZoneGetNextDaylightSavingTimeTransition(\_:\_:) 

Function

# CFTimeZoneGetNextDaylightSavingTimeTransition(\_:\_:)

Returns the time in a given time zone of the next daylight saving time transition after a given time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFTimeZoneGetNextDaylightSavingTimeTransition(
    _ tz: CFTimeZone!,
    _ at: CFAbsoluteTime
) -> CFAbsoluteTime
```

## Parameters 

`tz`  

The time zone to analyze.

`at`  

A time in `tz`.

## Return Value

The time in `tz` of the next daylight saving time transition after `at`.

## See Also

### Getting Daylight Savings Time Information

func CFTimeZoneIsDaylightSavingTime(CFTimeZone!, CFAbsoluteTime) -> Bool

Returns whether or not a time zone is in daylight savings time at a specified date.

func CFTimeZoneGetDaylightSavingTimeOffset(CFTimeZone!, CFAbsoluteTime) -> CFTimeInterval

Returns the daylight saving time offset for a time zone at a given time.

