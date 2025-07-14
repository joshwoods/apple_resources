

- Core Foundation
- CFLocaleKey
-  alternateQuotationEndDelimiterKey 

Type Property

# alternateQuotationEndDelimiterKey

Specifies the alternating end quotation symbol associated with the locale. In some locales, when quotations are nested, the quotation characters alternate. Thus, `NSLocaleQuotationEndDelimiterKey`, then `NSLocaleAlternateQuotationEndDelimiterKey`, and so on.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let alternateQuotationEndDelimiterKey: CFLocaleKey!
```

## Discussion

The corresponding value is a CFString object.

## See Also

### Constants

static let identifier: CFLocaleKey!

Specifies locale identifier.

static let languageCode: CFLocaleKey!

Specifies the locale language code.

static let countryCode: CFLocaleKey!

Specifies the locale country code.

static let scriptCode: CFLocaleKey!

Specifies the locale script code.

static let variantCode: CFLocaleKey!

Specifies the locale variant code.

static let exemplarCharacterSet: CFLocaleKey!

Specifies the locale character set.

static let calendarIdentifier: CFLocaleKey!

Specifies the locale calendar identifier.

static let calendar: CFLocaleKey!

Specifies the locale calendar.

static let collationIdentifier: CFLocaleKey!

Specifies the locale collation identifier.

static let usesMetricSystem: CFLocaleKey!

Specifies the whether the locale uses the metric system.

static let measurementSystem: CFLocaleKey!

Specifies the measurement system used.

static let decimalSeparator: CFLocaleKey!

Specifies the decimal point string.

static let groupingSeparator: CFLocaleKey!

Specifies the separator string between groups of digits.

static let currencySymbol: CFLocaleKey!

Specifies the currency symbol.

static let currencyCode: CFLocaleKey!

Specifies the locale currency code.

