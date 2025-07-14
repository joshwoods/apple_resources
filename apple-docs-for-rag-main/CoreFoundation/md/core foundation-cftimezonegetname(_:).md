

- Core Foundation
-  CFTimeZoneGetName(\_:) 

Function

# CFTimeZoneGetName(\_:)

Returns the geopolitical region name that identifies a given time zone.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTimeZoneGetName(_ tz: CFTimeZone!) -> CFString!
```

## Parameters 

`tz`  

The time zone to analyze.

## Return Value

A string containing the geopolitical region name that identifies `tz`. Ownership follows the The Get Rule.

## See Also

### Getting Information About Time Zones

func CFTimeZoneCopyLocalizedName(CFTimeZone!, CFTimeZoneNameStyle, CFLocale!) -> CFString!

Returns the localized name of a given time zone.

func CFTimeZoneGetSecondsFromGMT(CFTimeZone!, CFAbsoluteTime) -> CFTimeInterval

Returns the difference in seconds between the receiver and Greenwich Mean Time (GMT) at the specified date.

func CFTimeZoneGetData(CFTimeZone!) -> CFData!

Returns the data that stores the information used by a time zone.

