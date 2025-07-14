

- Core Foundation
-  CFTimeZoneCopyDefault() 

Function

# CFTimeZoneCopyDefault()

Returns the default time zone set for your application.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTimeZoneCopyDefault() -> CFTimeZone!
```

## Return Value

A time zone representing the default time zone set for your application, or the system time zone if no default is set. Ownership follows the The Create Rule.

## Discussion

If no default time zone is set, this function simply returns the result of the CFTimeZoneCopySystem() function.

## See Also

### System and Default Time Zones and Information

func CFTimeZoneCopyAbbreviationDictionary() -> CFDictionary!

Returns a dictionary holding the mappings of time zone abbreviations to time zone names.

func CFTimeZoneCopyAbbreviation(CFTimeZone!, CFAbsoluteTime) -> CFString!

Returns the abbreviation of a time zone at a specified date.

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

