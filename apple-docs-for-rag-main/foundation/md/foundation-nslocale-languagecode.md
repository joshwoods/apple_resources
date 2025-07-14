

- Foundation
- NSLocale
-  languageCode 

Instance Property

# languageCode

The language code for the locale.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var languageCode: String { get }
```

## Discussion

Examples of language codes include `"en"`, `"es"`, and `"zh"`.

Use localizedString(forLanguageCode:) to obtain a version of the value suitable for display to the user.

This property contains the same value returned by the object(forKey:) method when passing the languageCode key.

## See Also

### Related Documentation

class var isoLanguageCodes: [String]

The list of known language codes.

### Getting Information About a Locale

var localeIdentifier: String

The identifier for the locale.

var countryCode: String?

The country or region code for the locale.

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

