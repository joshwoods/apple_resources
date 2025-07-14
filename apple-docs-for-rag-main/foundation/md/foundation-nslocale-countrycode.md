

- Foundation
- NSLocale
-  countryCode 

Instance Property

# countryCode

The country or region code for the locale.

iOS 10.0–18.4DeprecatediPadOS 10.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.12–15.4DeprecatedtvOS 10.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 3.0–9.0Deprecated

``` source
var countryCode: String? { get }
```

## Discussion

Examples of country or region codes include `"GB"`, `"FR"`, and `"HK"`.

Use localizedString(forCountryCode:) to obtain a version of the value suitable for display to the user.

This property contains the same value returned by the object(forKey:) method when passing the countryCode key.

## See Also

### Related Documentation

class var isoCountryCodes: [String]

The list of known country or region codes.

### Getting Information About a Locale

var localeIdentifier: String

The identifier for the locale.

var languageCode: String

The language code for the locale.

var scriptCode: String?

The script code for the locale.

var variantCode: String?

The variant code for the locale.

var exemplarCharacterSet: CharacterSet

The exemplar character set for the locale.

var collationIdentifier: String?

The collation identifier for the locale.

var collatorIdentifier: String

The collator identifier for the locale.

var usesMetricSystem: Bool

A Boolean value that indicates whether the locale uses the metric system.

var decimalSeparator: String

The decimal separator for the locale.

var groupingSeparator: String

The grouping separator for the locale.

var currencyCode: String?

The currency code for the locale.

var currencySymbol: String

The currency symbol for the locale.

var calendarIdentifier: String

The calendar identifier for the locale.

var quotationBeginDelimiter: String

The begin quotation symbol for the locale.

var quotationEndDelimiter: String

The end quotation symbol for the locale.

