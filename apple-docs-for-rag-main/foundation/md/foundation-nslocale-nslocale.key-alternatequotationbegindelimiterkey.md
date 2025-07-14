

- Foundation
- NSLocale
- NSLocale.Key
-  alternateQuotationBeginDelimiterKey 

Type Property

# alternateQuotationBeginDelimiterKey

The alternating begin quotation symbol associated with the locale.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let alternateQuotationBeginDelimiterKey: NSLocale.Key
```

## Discussion

The corresponding value is an `NSString` object; for example, `"‘"`, `"‹"`, or `"『"`.

In some locales, when quotations are nested, the quotation characters alternate. Thus, quotationBeginDelimiterKey, then alternateQuotationBeginDelimiterKey, etc.

## See Also

### Keys

static let identifier: NSLocale.Key

The locale identifier.

static let countryCode: NSLocale.Key

The locale country or region code.

static let languageCode: NSLocale.Key

The locale language code.

static let scriptCode: NSLocale.Key

The locale script code.

static let variantCode: NSLocale.Key

The locale variant code.

static let exemplarCharacterSet: NSLocale.Key

The exemplar character set for the locale.

static let calendar: NSLocale.Key

The calendar associated with the locale.

static let collationIdentifier: NSLocale.Key

The collation associated with the locale.

static let collatorIdentifier: NSLocale.Key

The collation identifier for the locale.

static let usesMetricSystem: NSLocale.Key

A flag that indicates whether the locale uses the metric system.

static let measurementSystem: NSLocale.Key

The measurement system associated with the locale.

static let decimalSeparator: NSLocale.Key

The decimal separator associated with the locale.

static let groupingSeparator: NSLocale.Key

The numeric grouping separator associated with the locale.

static let currencySymbol: NSLocale.Key

The currency symbol associated with the locale.

static let currencyCode: NSLocale.Key

The currency code associated with the locale.

