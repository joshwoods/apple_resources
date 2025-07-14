

- Core Foundation
-  CFLocaleCreateLocaleIdentifierFromComponents(\_:\_:) 

Function

# CFLocaleCreateLocaleIdentifierFromComponents(\_:\_:)

Returns a locale identifier consisting of language, script, country or region, variant, and keyword/value pairs derived from a dictionary containing the source information.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFLocaleCreateLocaleIdentifierFromComponents(
    _ allocator: CFAllocator!,
    _ dictionary: CFDictionary!
) -> CFLocaleIdentifier!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`dictionary`  

The dictionary to use when creating the locale identifier.

## Return Value

A locale identifier consisting of language, script, country or region, variant, and keyword/value pairs derived from `dictionary`. Returns `NULL` if there was a problem creating the string. Ownership follows the The Create Rule.

## Discussion

Reverses the actions of CFLocaleCreateComponentsFromLocaleIdentifier(_:_:), creating a single string from the data in the specified dictionary. For example, the dictionary {``` kCFLocaleLanguageCode``=en``, ``` ``` kCFLocaleCountryCode``=US``, ``` ``` kCFLocaleCalendarIdentifier``=``kCFJapaneseCalendar``} ``` becomes `"en_US@calendar=japanese"`.

## See Also

### Getting and Creating Locale Identifiers

func CFLocaleCreateCanonicalLocaleIdentifierFromScriptManagerCodes(CFAllocator!, LangCode, RegionCode) -> CFLocaleIdentifier!

Returns a canonical locale identifier from given language and region codes.

func CFLocaleCreateCanonicalLanguageIdentifierFromString(CFAllocator!, CFString!) -> CFLocaleIdentifier!

Returns a canonical language identifier by mapping an arbitrary locale identification string to the canonical identifier

func CFLocaleCreateCanonicalLocaleIdentifierFromString(CFAllocator!, CFString!) -> CFLocaleIdentifier!

Returns a canonical locale identifier by mapping an arbitrary locale identification string to the canonical identifier.

func CFLocaleCreateComponentsFromLocaleIdentifier(CFAllocator!, CFLocaleIdentifier!) -> CFDictionary!

Returns a dictionary containing the result from parsing a locale ID consisting of language, script, country or region, variant, and keyword/value pairs.

func CFLocaleCreateLocaleIdentifierFromWindowsLocaleCode(CFAllocator!, UInt32) -> CFLocaleIdentifier!

Returns a locale identifier from a Windows locale code.

func CFLocaleGetWindowsLocaleCodeFromLocaleIdentifier(CFLocaleIdentifier!) -> UInt32

Returns a Windows locale code from the locale identifier.

