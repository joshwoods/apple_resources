

- Foundation
- NSLocale
-  localizedString(forCurrencyCode:) 

Instance Method

# localizedString(forCurrencyCode:)

Returns the localized string for the specified currency code.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func localizedString(forCurrencyCode currencyCode: String) -> String?
```

## Parameters 

`currencyCode`  

The code for the currency whose name you want.

## Return Value

The localized name of the currency.

## Discussion

For example, calling this method on an American English (`en_US`) locale, passing `"JPY"` for `currencyCode`, produces the string `"Japanese Yen"`.

This method is equivalent to calling the displayName(forKey:value:) method passing the currencyCode key and `currencyCode` value.

## See Also

### Getting Display Information About a Locale

func localizedString(forLocaleIdentifier: String) -> String

Returns the localized string for the specified locale identifier.

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

func localizedString(forCalendarIdentifier: String) -> String?

Returns the localized string for the specified calendar identifier.

Locale Calendar Identifiers

The types of calendars.

