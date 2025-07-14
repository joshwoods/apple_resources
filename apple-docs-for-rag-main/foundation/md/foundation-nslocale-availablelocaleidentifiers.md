

- Foundation
- NSLocale
-  availableLocaleIdentifiers 

Type Property

# availableLocaleIdentifiers

The list of locale identifiers available on the system.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var availableLocaleIdentifiers: [String] { get }
```

## Discussion

A locale identifier starts with a language code, often includes a region code, and occasionally includes a script designator. See Locale IDs for more information about the structure of a locale identifier.

Use localizedString(forLocaleIdentifier:) to obtain a human readable description of any of the locale identifiers in this list.

## See Also

### Related Documentation

Internationalization and Localization Guide

### Getting Known Identifiers and Codes

class var isoCountryCodes: [String]

The list of known country or region codes.

class var isoLanguageCodes: [String]

The list of known language codes.

class var isoCurrencyCodes: [String]

The list of known currency codes.

class var commonISOCurrencyCodes: [String]

A list of commonly encountered currency codes.

