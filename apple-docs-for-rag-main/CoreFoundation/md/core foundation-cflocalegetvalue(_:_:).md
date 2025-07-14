

- Core Foundation
-  CFLocaleGetValue(\_:\_:) 

Function

# CFLocaleGetValue(\_:\_:)

Returns the corresponding value for the given key of a locale’s key-value pair.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFLocaleGetValue(
    _ locale: CFLocale!,
    _ key: CFLocaleKey!
) -> CFTypeRef!
```

## Parameters 

`locale`  

The locale object to examine.

`key`  

The key for which to obtain the corresponding value. Possible values are described in Locale Property Keys.

## Return Value

The value corresponding to the given key in locale. The value may be any type of CFType object. Ownership follows the The Get Rule.

## Discussion

Locale objects use key-value pairs to store property values. Use this function to get the value of a specific property.

## See Also

### Getting Information About a Locale

func CFLocaleCopyDisplayNameForPropertyValue(CFLocale!, CFLocaleKey!, CFString!) -> CFString!

Returns the display name for the given value.

func CFLocaleGetIdentifier(CFLocale!) -> CFLocaleIdentifier!

Returns the given locale’s identifier.

