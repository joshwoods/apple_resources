

- Core Foundation
-  CFLocaleGetSystem() 

Function

# CFLocaleGetSystem()

Returns the root, canonical locale.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFLocaleGetSystem() -> CFLocale!
```

## Return Value

The root, canonical locale. Ownership follows the The Get Rule.

## Discussion

The root locale contains fixed backstop settings for all locale information.

## See Also

### Creating a Locale

func CFLocaleCopyCurrent() -> CFLocale!

Returns a copy of the logical locale for the current user.

func CFLocaleCreate(CFAllocator!, CFLocaleIdentifier!) -> CFLocale!

Creates a locale for the given arbitrary locale identifier.

func CFLocaleCreateCopy(CFAllocator!, CFLocale!) -> CFLocale!

Returns a copy of a locale.

