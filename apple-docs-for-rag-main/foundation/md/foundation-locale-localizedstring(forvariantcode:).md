

- Foundation
- Locale
-  localizedString(forVariantCode:) 

Instance Method

# localizedString(forVariantCode:)

Returns a localized string for a specified variant code.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func localizedString(forVariantCode variantCode: String) -> String?
```

## Discussion

For example, in the “en” locale, the result for `"POSIX"` is `"Computer"`.

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

func localizedString(forRegionCode: String) -> String?

Returns a localized string for a specified region code.

func localizedString(forScriptCode: String) -> String?

Returns a localized string for a specified script code.

