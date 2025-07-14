

- Core Foundation
-  CFTimeZoneCopyKnownNames() 

Function

# CFTimeZoneCopyKnownNames()

Returns an array of strings containing the names of all the time zones known to the system.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTimeZoneCopyKnownNames() -> CFArray!
```

## Return Value

An array containing CFString objects representing all the known time zone names. Ownership follows the The Create Rule.

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

func CFTimeZoneResetSystem()

Clears the previously determined system time zone, if any.

func CFTimeZoneSetAbbreviationDictionary(CFDictionary!)

Sets the abbreviation dictionary to a given dictionary.

