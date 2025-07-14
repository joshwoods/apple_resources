

- Core Foundation
-  CFTimeZoneGetData(\_:) 

Function

# CFTimeZoneGetData(\_:)

Returns the data that stores the information used by a time zone.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTimeZoneGetData(_ tz: CFTimeZone!) -> CFData!
```

## Parameters 

`tz`  

The time zone to analyze.

## Return Value

The data used to store `tz`. Ownership follows the The Get Rule. May be `NULL` if the timezone does not have any data or use Olson data for its information.

## See Also

### Getting Information About Time Zones

func CFTimeZoneGetName(CFTimeZone!) -> CFString!

Returns the geopolitical region name that identifies a given time zone.

func CFTimeZoneCopyLocalizedName(CFTimeZone!, CFTimeZoneNameStyle, CFLocale!) -> CFString!

Returns the localized name of a given time zone.

func CFTimeZoneGetSecondsFromGMT(CFTimeZone!, CFAbsoluteTime) -> CFTimeInterval

Returns the difference in seconds between the receiver and Greenwich Mean Time (GMT) at the specified date.

