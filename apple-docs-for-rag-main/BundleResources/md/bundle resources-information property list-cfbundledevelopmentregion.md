

- Bundle Resources
- Information Property List
-  CFBundleDevelopmentRegion 

Property List Key

# CFBundleDevelopmentRegion

The default language and region for the bundle, as a language ID.

iOS 2.0+iPadOS 2.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

## Details 

Name  
Localization native development region

Type  

string

## Attributes 

Default: `en-US`

## Discussion

The system uses this key as the language if it can’t locate a resource for the user’s preferred language. The value should be a *language ID* that identifies a language, dialect, or script.

### Languages

For a language used in many regions, use a code that represents a language designator. To specify English, use the en language designator. Use the two-letter ISO 639-1 standard (preferred) or the three-letter ISO 639-2 standard. If an ISO 639-1 code isn’t available for a particular language, use the ISO 639-2 code instead. There’s no ISO 639-1 code for the Hawaiian language, so use the ISO 639-2 code.

### Dialects

To distinguish between different languages and regional dialects, use a language designator with a region designator and a script designator separated by hyphens. To specify the English language as it’s used in the United Kingdom, use en-GB, where GB is the region designator. To represent Mandarin Chinese, spoken in Taiwan, and written in Traditional Chinese script, use zh-Hant-TW.

To specify a script, combine a language designator with a script designator separated by a hyphen, as in az-Arab for Azerbaijani in the Arabic script.

## See Also

### Localization

CFBundleLocalizations

The localizations handled manually by your app.

**Name:** Localizations

CFBundleAllowMixedLocalizations

A Boolean value that indicates whether the bundle supports the retrieval of localized strings from frameworks.

**Name:** Localized resources can be mixed

TICapsLockLanguageSwitchCapable

A Boolean value that enables the Caps Lock key to switch between Latin and non-Latin input sources.

