

- Foundation
- NSLocale
-  localeIdentifier 

Instance Property

# localeIdentifier

The identifier for the locale.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var localeIdentifier: String { get }
```

## Discussion

Examples of locale identifiers include `"en_GB"`, `"es_ES_PREEURO"`, and `"zh-Hant_HK_POSIX@collation=pinyin;currency=CNY"`.

Use localizedString(forIdentifier:) to obtain a version of the value suitable for display to the user.

Note

The value held in the property may differ from the identifier used to initialize the locale because NSLocale may canonicalize it during initialization.

This property contains the same value returned by the object(forKey:) method when passing the identifier key.

## See Also

### Related Documentation

class var availableLocaleIdentifiers: [String]

The list of locale identifiers available on the system.

### Getting Information About a Locale

var countryCode: String?

The country or region code for the locale.

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

