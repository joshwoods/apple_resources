

- Foundation
- NSLocale
-  localizedString(forCollatorIdentifier:) 

Instance Method

# localizedString(forCollatorIdentifier:)

Returns the localized string for the specified collator identifier.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func localizedString(forCollatorIdentifier collatorIdentifier: String) -> String?
```

## Parameters 

`collatorIdentifier`  

The identifier for the collator whose name you want.

## Return Value

The localized name of the collator.

## Discussion

This method is equivalent to calling the displayName(forKey:value:) method passing the collatorIdentifier key and `collatorIdentifier` value.

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

func localizedString(forCurrencyCode: String) -> String?

Returns the localized string for the specified currency code.

func localizedString(forCalendarIdentifier: String) -> String?

Returns the localized string for the specified calendar identifier.

Locale Calendar Identifiers

The types of calendars.

