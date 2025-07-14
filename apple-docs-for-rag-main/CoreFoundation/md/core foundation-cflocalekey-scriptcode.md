

- Core Foundation
- CFLocaleKey
-  scriptCode 

Type Property

# scriptCode

Specifies the locale script code.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let scriptCode: CFLocaleKey!
```

## Discussion

The corresponding value is a CFString containing a Unicode script tag (strictly, an ISO 15924 script tag). Usually this is empty (it is for “`ja_JP`”). It may be present for locales where a script *must* be specified, for example “`uz-Latn-UZ`” vs. “`uz-Cyrl-UZ`” for Uzbek in Latin vs. Cyrillic (in the first case the script code is “`Latn`”, and in the second it is “`Cyrl`”).

## See Also

### Constants

static let identifier: CFLocaleKey!

Specifies locale identifier.

static let languageCode: CFLocaleKey!

Specifies the locale language code.

static let countryCode: CFLocaleKey!

Specifies the locale country code.

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

