

- Core Foundation
-  CFLocaleCreate(\_:\_:) 

Function

# CFLocaleCreate(\_:\_:)

Creates a locale for the given arbitrary locale identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFLocaleCreate(
    _ allocator: CFAllocator!,
    _ localeIdentifier: CFLocaleIdentifier!
) -> CFLocale!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`localeIdentifier`  

A string representation of an arbitrary locale identifier.

## Return Value

A new locale that corresponds to the arbitrary locale identifier `localeIdentifier`. Returns `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### Creating a Locale

func CFLocaleCopyCurrent() -> CFLocale!

Returns a copy of the logical locale for the current user.

func CFLocaleCreateCopy(CFAllocator!, CFLocale!) -> CFLocale!

Returns a copy of a locale.

func CFLocaleGetSystem() -> CFLocale!

Returns the root, canonical locale.

