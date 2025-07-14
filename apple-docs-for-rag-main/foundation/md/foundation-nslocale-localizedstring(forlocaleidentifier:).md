

- Foundation
- NSLocale
-  localizedString(forLocaleIdentifier:) 

Instance Method

# localizedString(forLocaleIdentifier:)

Returns the localized string for the specified locale identifier.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func localizedString(forLocaleIdentifier localeIdentifier: String) -> String
```

## Parameters 

`localeIdentifier`  

The identifier for which you want the localized name.

## Return Value

The localized name of the locale.

## Discussion

For example, calling this method on an American English (`en_US`) locale, passing `"fr_FR"` for `localeIdentifier`, produces the string `"French (France)"`.

This method is equivalent to calling the displayName(forKey:value:) method passing the identifier key and `localeIdentifier` value.

## See Also

### Related Documentation

class var availableLocaleIdentifiers: [String]

The list of locale identifiers available on the system.

### Getting Display Information About a Locale

func localizedString(forCountryCode: String) -> String?

Returns the localized string for a country or region code.

func localizedString(forLanguageCode: String) -> String?

Returns the localized string for the specified language code.

func localizedString(forScriptCode: String) -> String?

Returns the localized string for the specified script code.

func localizedString(forVariantCode: String) -> String?

Returns the localized string for the specified variant code.

func localizedString(forCollationIdentifier: String) -> String?

Returns the localized string for the specified collation identifier.

func localizedString(forCollatorIdentifier: String) -> String?

Returns the localized string for the specified collator identifier.

func localizedString(forCurrencyCode: String) -> String?

Returns the localized string for the specified currency code.

func localizedString(forCalendarIdentifier: String) -> String?

Returns the localized string for the specified calendar identifier.

Locale Calendar Identifiers

The types of calendars.

