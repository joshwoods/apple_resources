

- Core Foundation
-  CFTimeZoneGetSecondsFromGMT(\_:\_:) 

Function

# CFTimeZoneGetSecondsFromGMT(\_:\_:)

Returns the difference in seconds between the receiver and Greenwich Mean Time (GMT) at the specified date.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTimeZoneGetSecondsFromGMT(
    _ tz: CFTimeZone!,
    _ at: CFAbsoluteTime
) -> CFTimeInterval
```

## Parameters 

`tz`  

The time zone to analyze.

`at`  

The date at which the interval is to be computed.

## Return Value

The difference in seconds between `tz` and GMT at the specified date, `at`.

## See Also

### Getting Information About Time Zones

func CFTimeZoneGetName(CFTimeZone!) -> CFString!

Returns the geopolitical region name that identifies a given time zone.

func CFTimeZoneCopyLocalizedName(CFTimeZone!, CFTimeZoneNameStyle, CFLocale!) -> CFString!

Returns the localized name of a given time zone.

func CFTimeZoneGetData(CFTimeZone!) -> CFData!

Returns the data that stores the information used by a time zone.

