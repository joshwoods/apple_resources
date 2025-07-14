

- Core Foundation
-  CFLocaleGetWindowsLocaleCodeFromLocaleIdentifier(\_:) 

Function

# CFLocaleGetWindowsLocaleCodeFromLocaleIdentifier(\_:)

Returns a Windows locale code from the locale identifier.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFLocaleGetWindowsLocaleCodeFromLocaleIdentifier(_ localeIdentifier: CFLocaleIdentifier!) -> UInt32
```

## Parameters 

`localeIdentifier`  

The locale identifier.

## Return Value

The Windows locale code.

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

func CFLocaleCreateLocaleIdentifierFromComponents(CFAllocator!, CFDictionary!) -> CFLocaleIdentifier!

Returns a locale identifier consisting of language, script, country or region, variant, and keyword/value pairs derived from a dictionary containing the source information.

func CFLocaleCreateLocaleIdentifierFromWindowsLocaleCode(CFAllocator!, UInt32) -> CFLocaleIdentifier!

Returns a locale identifier from a Windows locale code.

