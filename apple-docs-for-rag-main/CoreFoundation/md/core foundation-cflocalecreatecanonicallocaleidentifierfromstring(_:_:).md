

- Core Foundation
-  CFLocaleCreateCanonicalLocaleIdentifierFromString(\_:\_:) 

Function

# CFLocaleCreateCanonicalLocaleIdentifierFromString(\_:\_:)

Returns a canonical locale identifier by mapping an arbitrary locale identification string to the canonical identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFLocaleCreateCanonicalLocaleIdentifierFromString(
    _ allocator: CFAllocator!,
    _ localeIdentifier: CFString!
) -> CFLocaleIdentifier!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`localeIdentifier`  

A string representation of an arbitrary locale identifier (for example, “English”).

## Return Value

A canonical locale identifier created by mapping the arbitrary locale identification string to the canonical identifier for the corresponding locale (for example, “en”). Returns `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### Getting and Creating Locale Identifiers

func CFLocaleCreateCanonicalLocaleIdentifierFromScriptManagerCodes(CFAllocator!, LangCode, RegionCode) -> CFLocaleIdentifier!

Returns a canonical locale identifier from given language and region codes.

func CFLocaleCreateCanonicalLanguageIdentifierFromString(CFAllocator!, CFString!) -> CFLocaleIdentifier!

Returns a canonical language identifier by mapping an arbitrary locale identification string to the canonical identifier

func CFLocaleCreateComponentsFromLocaleIdentifier(CFAllocator!, CFLocaleIdentifier!) -> CFDictionary!

Returns a dictionary containing the result from parsing a locale ID consisting of language, script, country or region, variant, and keyword/value pairs.

func CFLocaleCreateLocaleIdentifierFromComponents(CFAllocator!, CFDictionary!) -> CFLocaleIdentifier!

Returns a locale identifier consisting of language, script, country or region, variant, and keyword/value pairs derived from a dictionary containing the source information.

func CFLocaleCreateLocaleIdentifierFromWindowsLocaleCode(CFAllocator!, UInt32) -> CFLocaleIdentifier!

Returns a locale identifier from a Windows locale code.

func CFLocaleGetWindowsLocaleCodeFromLocaleIdentifier(CFLocaleIdentifier!) -> UInt32

Returns a Windows locale code from the locale identifier.

