

- Core Foundation
-  CFTimeZoneCopyAbbreviationDictionary() 

Function

# CFTimeZoneCopyAbbreviationDictionary()

Returns a dictionary holding the mappings of time zone abbreviations to time zone names.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTimeZoneCopyAbbreviationDictionary() -> CFDictionary!
```

## Return Value

A dictionary containing the mappings of time zone abbreviations to time zone names. Ownership follows the The Create Rule.

## Discussion

More than one time zone may have the same abbreviation. For example, US/Pacific and Canada/Pacific both use the abbreviation “PST.” In these cases this function chooses a single name to map the abbreviation to.

## See Also

### System and Default Time Zones and Information

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

func CFTimeZoneSetAbbreviationDictionary(CFDictionary!)

Sets the abbreviation dictionary to a given dictionary.

