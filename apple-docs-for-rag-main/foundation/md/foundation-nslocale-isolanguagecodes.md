

- Foundation
- NSLocale
-  isoLanguageCodes 

Type Property

# isoLanguageCodes

The list of known language codes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var isoLanguageCodes: [String] { get }
```

## Discussion

A language code is a short string that represent a particular language. All languages have a three-character ISO 639-2 string, while some languages also have a two-character ISO 639-1 string. See ISO 639.2 Codes for the Representation of Names of Languages for the complete list of standardized language codes.

The array provided by this property contains a list of codes for all the languages the system knows about, designated by the ISO 639-1 code if available, or the ISO 639-2 code if not. Use the method localizedString(forLanguageCode:) to obtain a human readable string for any of the codes in the list.

For more information about language localization in your app, see Language and Locale IDs.

Not all language codes have supporting locale data in the system.

## See Also

### Getting Known Identifiers and Codes

class var availableLocaleIdentifiers: [String]

The list of locale identifiers available on the system.

class var isoCountryCodes: [String]

The list of known country or region codes.

class var isoCurrencyCodes: [String]

The list of known currency codes.

class var commonISOCurrencyCodes: [String]

A list of commonly encountered currency codes.

