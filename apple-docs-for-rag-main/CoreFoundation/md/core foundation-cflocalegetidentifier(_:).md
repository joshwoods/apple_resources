

- Core Foundation
-  CFLocaleGetIdentifier(\_:) 

Function

# CFLocaleGetIdentifier(\_:)

Returns the given locale’s identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFLocaleGetIdentifier(_ locale: CFLocale!) -> CFLocaleIdentifier!
```

## Parameters 

`locale`  

The locale object to examine.

## Return Value

A string representation of `locale`’s identifier. This may not be the same string that was used to create the locale—it may be canonicalized. Ownership follows the The Get Rule.

## See Also

### Getting Information About a Locale

func CFLocaleCopyDisplayNameForPropertyValue(CFLocale!, CFLocaleKey!, CFString!) -> CFString!

Returns the display name for the given value.

func CFLocaleGetValue(CFLocale!, CFLocaleKey!) -> CFTypeRef!

Returns the corresponding value for the given key of a locale’s key-value pair.

