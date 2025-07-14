

- Core Foundation
-  CFTimeZoneCopyAbbreviation(\_:\_:) 

Function

# CFTimeZoneCopyAbbreviation(\_:\_:)

Returns the abbreviation of a time zone at a specified date.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTimeZoneCopyAbbreviation(
    _ tz: CFTimeZone!,
    _ at: CFAbsoluteTime
) -> CFString!
```

## Parameters 

`tz`  

The time zone to use.

`at`  

The absolute time at which to obtain the abbreviation.

## Return Value

A string containing the time zone abbreviation of `at`. Ownership follows the The Create Rule.

## Discussion

Note that the abbreviation may be different at different dates. For example, during daylight savings time the US/Eastern time zone has an abbreviation of “EDT.” At other times, its abbreviation is “EST.”

## See Also

### System and Default Time Zones and Information

func CFTimeZoneCopyAbbreviationDictionary() -> CFDictionary!

Returns a dictionary holding the mappings of time zone abbreviations to time zone names.

func CFTimeZoneCopyDefault() -> CFTimeZone!

Returns the default time zone set for your application.

func CFTimeZoneCopySystem() -> CFTimeZone!

Returns the time zone currently used by the system.

func CFTimeZoneSetDefault(CFTimeZone!)

Sets the default time zone for your application the given time zone.

func CFTimeZoneCopyKnownNames() -> CFArray!

Returns an array of strings containing the names of all the time zones known to the system.

func CFTimeZoneResetSystem()

Clears the previously determined system time zone, if any.

func CFTimeZoneSetAbbreviationDictionary(CFDictionary!)

Sets the abbreviation dictionary to a given dictionary.

