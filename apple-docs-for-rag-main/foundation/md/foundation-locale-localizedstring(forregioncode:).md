

- Foundation
- Locale
-  localizedString(forRegionCode:) 

Instance Method

# localizedString(forRegionCode:)

Returns a localized string for a specified region code.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func localizedString(forRegionCode regionCode: String) -> String?
```

## Discussion

For example, in the “en” locale, the result for `"fr"` is `"France"`.

## See Also

### Getting display information about a locale

func localizedString(for: Calendar.Identifier) -> String?

Returns a localized string for a specified calendar.

func localizedString(forCollationIdentifier: String) -> String?

Returns a localized string for a specified ICU collation identifier.

func localizedString(forCollatorIdentifier: String) -> String?

Returns a localized string for a specified ICU collator identifier.

func localizedString(forCurrencyCode: String) -> String?

Returns a localized string for a specified ISO 4217 currency code.

func localizedString(forIdentifier: String) -> String?

Returns a localized string for a specified locale identifier.

func localizedString(forLanguageCode: String) -> String?

Returns a localized string for a specified language code.

func localizedString(forScriptCode: String) -> String?

Returns a localized string for a specified script code.

func localizedString(forVariantCode: String) -> String?

Returns a localized string for a specified variant code.

