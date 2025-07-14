

- Core Foundation
-  CFTimeZoneCopyLocalizedName(\_:\_:\_:) 

Function

# CFTimeZoneCopyLocalizedName(\_:\_:\_:)

Returns the localized name of a given time zone.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFTimeZoneCopyLocalizedName(
    _ tz: CFTimeZone!,
    _ style: CFTimeZoneNameStyle,
    _ locale: CFLocale!
) -> CFString!
```

## Parameters 

`tz`  

The time zone to analyze.

`style`  

The style for the returned name.

`locale`  

The locale for which to localize the returned name.

## Return Value

The name of `tz` localized for `locale`. Ownership follows the The Create Rule.

## See Also

### Getting Information About Time Zones

func CFTimeZoneGetName(CFTimeZone!) -> CFString!

Returns the geopolitical region name that identifies a given time zone.

func CFTimeZoneGetSecondsFromGMT(CFTimeZone!, CFAbsoluteTime) -> CFTimeInterval

Returns the difference in seconds between the receiver and Greenwich Mean Time (GMT) at the specified date.

func CFTimeZoneGetData(CFTimeZone!) -> CFData!

Returns the data that stores the information used by a time zone.

