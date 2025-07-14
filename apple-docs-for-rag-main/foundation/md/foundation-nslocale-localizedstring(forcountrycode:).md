

- Foundation
- NSLocale
-  localizedString(forCountryCode:) 

Instance Method

# localizedString(forCountryCode:)

Returns the localized string for a country or region code.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func localizedString(forCountryCode countryCode: String) -> String?
```

## Parameters 

`countryCode`  

The code of the country or region that indicates the name you want.

## Return Value

The localized name of the country or region.

## Discussion

For example, calling this method on an American English (`en_US`) locale, passing `"GB"` for `countryCode`, produces the string `"United Kingdom"`.

This method is equivalent to calling the displayName(forKey:value:) method passing the countryCode key and `countryCode` value.

## See Also

### Related Documentation

class var isoCountryCodes: [String]

The list of known country or region codes.

### Getting Display Information About a Locale

func localizedString(forLocaleIdentifier: String) -> String

Returns the localized string for the specified locale identifier.

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

