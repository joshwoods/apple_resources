

- Core Foundation
-  CFLocaleCreateComponentsFromLocaleIdentifier(\_:\_:) 

Function

# CFLocaleCreateComponentsFromLocaleIdentifier(\_:\_:)

Returns a dictionary containing the result from parsing a locale ID consisting of language, script, country or region, variant, and keyword/value pairs.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFLocaleCreateComponentsFromLocaleIdentifier(
    _ allocator: CFAllocator!,
    _ localeID: CFLocaleIdentifier!
) -> CFDictionary!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or `kCFAllocatorDefault` to use the current default allocator.

`localeID`  

The locale ID to use when creating the locale dictionary.

## Return Value

A dictionary containing the result from parsing a locale ID consisting of language, script, country or region, variant, and keyword/value pairs. Returns `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## Discussion

The dictionary keys are the constant CFString objects that correspond to the locale ID components; the values correspond to constants where available. For example: the string “en_US@calendar=japanese” yields a dictionary with three entries: ``` kCFLocaleLanguageCode``=en ```, ``` kCFLocaleCountryCode``=US ```, and ``` kCFLocaleCalendarIdentifier``=``kCFJapaneseCalendar ```. See also CFLocaleCreateLocaleIdentifierFromComponents(_:_:).

## See Also

### Getting and Creating Locale Identifiers

func CFLocaleCreateCanonicalLocaleIdentifierFromScriptManagerCodes(CFAllocator!, LangCode, RegionCode) -> CFLocaleIdentifier!

Returns a canonical locale identifier from given language and region codes.

func CFLocaleCreateCanonicalLanguageIdentifierFromString(CFAllocator!, CFString!) -> CFLocaleIdentifier!

Returns a canonical language identifier by mapping an arbitrary locale identification string to the canonical identifier

func CFLocaleCreateCanonicalLocaleIdentifierFromString(CFAllocator!, CFString!) -> CFLocaleIdentifier!

Returns a canonical locale identifier by mapping an arbitrary locale identification string to the canonical identifier.

func CFLocaleCreateLocaleIdentifierFromComponents(CFAllocator!, CFDictionary!) -> CFLocaleIdentifier!

Returns a locale identifier consisting of language, script, country or region, variant, and keyword/value pairs derived from a dictionary containing the source information.

func CFLocaleCreateLocaleIdentifierFromWindowsLocaleCode(CFAllocator!, UInt32) -> CFLocaleIdentifier!

Returns a locale identifier from a Windows locale code.

func CFLocaleGetWindowsLocaleCodeFromLocaleIdentifier(CFLocaleIdentifier!) -> UInt32

Returns a Windows locale code from the locale identifier.

