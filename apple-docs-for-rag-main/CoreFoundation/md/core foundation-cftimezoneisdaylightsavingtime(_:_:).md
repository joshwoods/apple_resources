

- Core Foundation
-  CFTimeZoneIsDaylightSavingTime(\_:\_:) 

Function

# CFTimeZoneIsDaylightSavingTime(\_:\_:)

Returns whether or not a time zone is in daylight savings time at a specified date.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTimeZoneIsDaylightSavingTime(
    _ tz: CFTimeZone!,
    _ at: CFAbsoluteTime
) -> Bool
```

## Parameters 

`tz`  

The time zone to analyze.

`at`  

The date in `tz` to test for daylight savings.

## Return Value

`true` if `tz` is in daylight savings time at `at`, otherwise `false`.

## See Also

### Getting Daylight Savings Time Information

func CFTimeZoneGetDaylightSavingTimeOffset(CFTimeZone!, CFAbsoluteTime) -> CFTimeInterval

Returns the daylight saving time offset for a time zone at a given time.

func CFTimeZoneGetNextDaylightSavingTimeTransition(CFTimeZone!, CFAbsoluteTime) -> CFAbsoluteTime

Returns the time in a given time zone of the next daylight saving time transition after a given time.

