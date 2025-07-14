

- Foundation
- NSLocale
-  NSLocale.Key 

Structure

# NSLocale.Key

The keys used to access components of a locale.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Key
```

## Discussion

Use these keys with the methods object(forKey:) and displayName(forKey:value:).

## Topics

### Initializers

init(rawValue: String)

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

static let quotationEndDelimiterKey: NSLocale.Key

The end quotation symbol associated with the locale.

static let quotationBeginDelimiterKey: NSLocale.Key

The begin quotation symbol associated with the locale.

static let alternateQuotationEndDelimiterKey: NSLocale.Key

The alternate end quotation symbol associated with the locale.

static let alternateQuotationBeginDelimiterKey: NSLocale.Key

The alternating begin quotation symbol associated with the locale.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Locale Information by Key

func object(forKey: NSLocale.Key) -> Any?

Returns the value of the component corresponding to the specified key.

func displayName(forKey: NSLocale.Key, value: Any) -> String?

Returns the display name for the given locale component value.

