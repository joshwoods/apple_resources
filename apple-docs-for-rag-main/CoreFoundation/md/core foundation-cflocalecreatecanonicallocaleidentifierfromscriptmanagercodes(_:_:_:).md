

- Core Foundation
-  CFLocaleCreateCanonicalLocaleIdentifierFromScriptManagerCodes(\_:\_:\_:) 

Function

# CFLocaleCreateCanonicalLocaleIdentifierFromScriptManagerCodes(\_:\_:\_:)

Returns a canonical locale identifier from given language and region codes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFLocaleCreateCanonicalLocaleIdentifierFromScriptManagerCodes(
    _ allocator: CFAllocator!,
    _ lcode: LangCode,
    _ rcode: RegionCode
) -> CFLocaleIdentifier!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`lcode`  

A macOS language code.

`rcode`  

A macOS region code.

## Return Value

A canonical locale identifier created by mapping `lcode` and `rcode` to a locale. Returns `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### Getting and Creating Locale Identifiers

func CFLocaleCreateCanonicalLanguageIdentifierFromString(CFAllocator!, CFString!) -> CFLocaleIdentifier!

Returns a canonical language identifier by mapping an arbitrary locale identification string to the canonical identifier

func CFLocaleCreateCanonicalLocaleIdentifierFromString(CFAllocator!, CFString!) -> CFLocaleIdentifier!

Returns a canonical locale identifier by mapping an arbitrary locale identification string to the canonical identifier.

func CFLocaleCreateComponentsFromLocaleIdentifier(CFAllocator!, CFLocaleIdentifier!) -> CFDictionary!

Returns a dictionary containing the result from parsing a locale ID consisting of language, script, country or region, variant, and keyword/value pairs.

func CFLocaleCreateLocaleIdentifierFromComponents(CFAllocator!, CFDictionary!) -> CFLocaleIdentifier!

Returns a locale identifier consisting of language, script, country or region, variant, and keyword/value pairs derived from a dictionary containing the source information.

func CFLocaleCreateLocaleIdentifierFromWindowsLocaleCode(CFAllocator!, UInt32) -> CFLocaleIdentifier!

Returns a locale identifier from a Windows locale code.

func CFLocaleGetWindowsLocaleCodeFromLocaleIdentifier(CFLocaleIdentifier!) -> UInt32

Returns a Windows locale code from the locale identifier.

