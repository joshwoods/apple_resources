

- Foundation
- NSLocale
-  localizedString(forVariantCode:) 

Instance Method

# localizedString(forVariantCode:)

Returns the localized string for the specified variant code.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func localizedString(forVariantCode variantCode: String) -> String?
```

## Parameters 

`variantCode`  

The variant code whose name you want.

## Return Value

The localized name of the variant.

## Discussion

For example, calling this method on an American English (`en_US`) locale, passing `"POSIX"` for `variantCode`, produces the string `"Computer"`.

This method is equivalent to calling the displayName(forKey:value:) method passing the variantCode key and `variantCode` value.

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

