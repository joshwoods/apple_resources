

- Core Foundation
- CFLocaleKey
-  variantCode 

Type Property

# variantCode

Specifies the locale variant code.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let variantCode: CFLocaleKey!
```

## Discussion

The corresponding value is a CFString containing the variant name. The variant code is arbitrary and application-specific. ICU adds “`_EURO`” to its locale designations for locales that support the Euro currency. For “`en_US_POSIX`” the variant is “`POSIX`”, and for “`hy_AM_REVISED`” it is “`REVISED`”.

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

