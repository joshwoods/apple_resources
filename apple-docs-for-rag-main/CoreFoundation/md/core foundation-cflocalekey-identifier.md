

- Core Foundation
- CFLocaleKey
-  identifier 

Type Property

# identifier

Specifies locale identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let identifier: CFLocaleKey!
```

## Discussion

The corresponding value is a CFString containing the POSIX locale identifier as used by ICU, such as “`ja_JP`”. If you have a variant locale or a different currency or calendar, it can be as complex as “`en_US_POSIX@calendar=japanese;currency=EUR`” or “`az_Cyrl_AZ@calendar=buddhist;currency=JPY`”.

## See Also

### Constants

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

static let collatorIdentifier: CFLocaleKey!

Specifies the collation identifier for the locale.

