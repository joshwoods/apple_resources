

- Core Foundation
-  CFLocaleCopyDisplayNameForPropertyValue(\_:\_:\_:) 

Function

# CFLocaleCopyDisplayNameForPropertyValue(\_:\_:\_:)

Returns the display name for the given value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFLocaleCopyDisplayNameForPropertyValue(
    _ displayLocale: CFLocale!,
    _ key: CFLocaleKey!,
    _ value: CFString!
) -> CFString!
```

## Parameters 

`displayLocale`  

A locale object.

`key`  

A string that identifies the type that `value` is. It must be one of the standard locale property keys (see Locale Property Keys).

`value`  

The value for which the display name is required.

## Return Value

The display name for `value`. Returns `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## Discussion

Note that not all locale property keys have values with display name values.

## See Also

### Getting Information About a Locale

func CFLocaleGetValue(CFLocale!, CFLocaleKey!) -> CFTypeRef!

Returns the corresponding value for the given key of a locale’s key-value pair.

func CFLocaleGetIdentifier(CFLocale!) -> CFLocaleIdentifier!

Returns the given locale’s identifier.

