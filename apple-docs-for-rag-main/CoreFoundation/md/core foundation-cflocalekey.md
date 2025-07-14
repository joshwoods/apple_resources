

- Core Foundation
-  CFLocaleKey 

Structure

# CFLocaleKey

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFLocaleKey
```

## Topics

### Type Properties

static let alternateQuotationBeginDelimiterKey: CFLocaleKey!

Specifies the alternating begin quotation symbol associated with the locale. In some locales, when quotations are nested, the quotation characters alternate. Thus, `NSLocaleQuotationBeginDelimiterKey`, then `NSLocaleAlternateQuotationBeginDelimiterKey`, and so on.

static let alternateQuotationEndDelimiterKey: CFLocaleKey!

Specifies the alternating end quotation symbol associated with the locale. In some locales, when quotations are nested, the quotation characters alternate. Thus, `NSLocaleQuotationEndDelimiterKey`, then `NSLocaleAlternateQuotationEndDelimiterKey`, and so on.

static let calendar: CFLocaleKey!

Specifies the locale calendar.

static let calendarIdentifier: CFLocaleKey!

Specifies the locale calendar identifier.

static let collationIdentifier: CFLocaleKey!

Specifies the locale collation identifier.

static let collatorIdentifier: CFLocaleKey!

Specifies the collation identifier for the locale.

static let countryCode: CFLocaleKey!

Specifies the locale country code.

static let currencyCode: CFLocaleKey!

Specifies the locale currency code.

static let currencySymbol: CFLocaleKey!

Specifies the currency symbol.

static let decimalSeparator: CFLocaleKey!

Specifies the decimal point string.

static let exemplarCharacterSet: CFLocaleKey!

Specifies the locale character set.

static let groupingSeparator: CFLocaleKey!

Specifies the separator string between groups of digits.

static let identifier: CFLocaleKey!

Specifies locale identifier.

static let languageCode: CFLocaleKey!

Specifies the locale language code.

static let measurementSystem: CFLocaleKey!

Specifies the measurement system used.

static let quotationBeginDelimiterKey: CFLocaleKey!

Specifies the begin quotation symbol associated with the locale.

static let quotationEndDelimiterKey: CFLocaleKey!

Specifies the end quotation symbol associated with the locale.

static let scriptCode: CFLocaleKey!

Specifies the locale script code.

static let usesMetricSystem: CFLocaleKey!

Specifies the whether the locale uses the metric system.

static let variantCode: CFLocaleKey!

Specifies the locale variant code.

### Initializers

init(rawValue: CFString)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Data Types

typealias CFAllocatorTypeID

struct CFCalendarIdentifier

struct CFDateFormatterKey

typealias CFErrorDomain

struct CFLocaleIdentifier

struct CFNotificationName

struct CFNumberFormatterKey

struct CFRunLoopMode

struct CFStreamPropertyKey

typealias CFTypeRef

An untyped “generic” reference to any Core Foundation object.

