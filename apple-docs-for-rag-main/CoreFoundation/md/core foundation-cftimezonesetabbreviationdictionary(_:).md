

- Core Foundation
-  CFTimeZoneSetAbbreviationDictionary(\_:) 

Function

# CFTimeZoneSetAbbreviationDictionary(\_:)

Sets the abbreviation dictionary to a given dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTimeZoneSetAbbreviationDictionary(_ dict: CFDictionary!)
```

## Parameters 

`dict`  

A dictionary containing key-value pairs for looking up time zone names given their abbreviations. The keys should be CFString objects containing the abbreviations; the values should be CFString objects containing their corresponding geopolitical region names.

## See Also

### System and Default Time Zones and Information

func CFTimeZoneCopyAbbreviationDictionary() -> CFDictionary!

Returns a dictionary holding the mappings of time zone abbreviations to time zone names.

func CFTimeZoneCopyAbbreviation(CFTimeZone!, CFAbsoluteTime) -> CFString!

Returns the abbreviation of a time zone at a specified date.

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

