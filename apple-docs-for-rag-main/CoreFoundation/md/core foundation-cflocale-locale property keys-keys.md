

- Core Foundation
- CFLocale
-  Locale Property Keys 

API Collection

# Locale Property Keys

Predefined locale keys used to get property values.

## Overview

Locale objects use key-value pairs to store property values. Use the CFLocaleGetValue(_:_:) function to get the value of a specific property listed above.

## Topics

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

static let collatorIdentifier: CFLocaleKey!

Specifies the collation identifier for the locale.

static let quotationBeginDelimiterKey: CFLocaleKey!

Specifies the begin quotation symbol associated with the locale.

static let quotationEndDelimiterKey: CFLocaleKey!

Specifies the end quotation symbol associated with the locale.

static let alternateQuotationBeginDelimiterKey: CFLocaleKey!

Specifies the alternating begin quotation symbol associated with the locale. In some locales, when quotations are nested, the quotation characters alternate. Thus, `NSLocaleQuotationBeginDelimiterKey`, then `NSLocaleAlternateQuotationBeginDelimiterKey`, and so on.

static let alternateQuotationEndDelimiterKey: CFLocaleKey!

Specifies the alternating end quotation symbol associated with the locale. In some locales, when quotations are nested, the quotation characters alternate. Thus, `NSLocaleQuotationEndDelimiterKey`, then `NSLocaleAlternateQuotationEndDelimiterKey`, and so on.

## See Also

### Constants

enum CFLocaleLanguageDirection

These constants describe the text direction for a language. They are returned by the functions CFLocaleGetLanguageCharacterDirection(_:) and CFLocaleGetLanguageLineDirection(_:).

Locale Calendar Identifiers

Predefined locale keys used to get calendar values—values for `kCFLocaleCalendarIdentifier`.

Locale Change Notification

Identifier for notification sent if the current locale changes.

