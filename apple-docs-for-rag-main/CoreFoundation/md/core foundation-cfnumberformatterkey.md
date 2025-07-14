

- Core Foundation
-  CFNumberFormatterKey 

Structure

# CFNumberFormatterKey

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFNumberFormatterKey
```

## Topics

### Type Properties

static let alwaysShowDecimalSeparator: CFNumberFormatterKey!

Specifies if the result of converting a value to a string should always contain the decimal separator, even if the number is an integer.

static let currencyCode: CFNumberFormatterKey!

Specifies the currency code, a `CFString` object.

static let currencyDecimalSeparator: CFNumberFormatterKey!

Specifies the currency decimal separator, a `CFString` object.

static let currencyGroupingSeparator: CFNumberFormatterKey!

Specifies the grouping symbol to use when placing a currency value within a string, a `CFString` object.

static let currencySymbol: CFNumberFormatterKey!

Specifies the symbol for the currency, a `CFString` object.

static let decimalSeparator: CFNumberFormatterKey!

Specifies the decimal separator, a `CFString` object.

static let defaultFormat: CFNumberFormatterKey!

The original format string for the formatter (given the date and time style and locale specified at creation), a `CFString` object.

static let exponentSymbol: CFNumberFormatterKey!

Specifies the exponent symbol (“E” or “e”) in the scientific notation of numbers (for example, as in `1.0e+56`), a `CFString` object.

static let formatWidth: CFNumberFormatterKey!

Specifies the width of a formatted number within a string that is either left justified or right justified based on the value of paddingPosition, a `CFNumber` object.

static let groupingSeparator: CFNumberFormatterKey!

Specifies the grouping separator, a `CFString` object.

static let groupingSize: CFNumberFormatterKey!

Specifies how often the “thousands” or grouping separator appears, as in “10,000,000”, a `CFNumber` object.

static let infinitySymbol: CFNumberFormatterKey!

Specifies the string that is used to represent the symbol for infinity, a `CFString` object.

static let internationalCurrencySymbol: CFNumberFormatterKey!

Specifies the international currency symbol to use when placing a formatted number within a string, a `CFString` object.

static let isLenient: CFNumberFormatterKey!

Specifies whether the formatter is lenient, a`CFBoolean` object.

static let maxFractionDigits: CFNumberFormatterKey!

Specifies the maximum number of digits after a decimal point, a `CFNumber` object.

static let maxIntegerDigits: CFNumberFormatterKey!

Specifies the maximum number of integer digits before a decimal point, a `CFNumber` object.

static let maxSignificantDigits: CFNumberFormatterKey!

Specifies the maximum number of significant digits to use, a`CFNumber` object.

static let minFractionDigits: CFNumberFormatterKey!

Specifies the minimum number of digits after a decimal point, a `CFNumber` object.

static let minIntegerDigits: CFNumberFormatterKey!

Specifies the minimum number of integer digits before a decimal point, a `CFNumber` object.

static let minSignificantDigits: CFNumberFormatterKey!

Specifies the minimum number of significant digits to use, a`CFNumber` object.

static let minusSign: CFNumberFormatterKey!

Specifies the symbol for the minus sign, a `CFString` object.

static let multiplier: CFNumberFormatterKey!

Specifies the multiplier to use when placing a formatted number within a string, a `CFNumber` object.

static let naNSymbol: CFNumberFormatterKey!

Specifies the string that is used to represent NaN (“not a number”) when values are converted to strings, a `CFString` object.

static let negativePrefix: CFNumberFormatterKey!

Specifies the minus sign prefix symbol to use when placing a formatted number within a string, a `CFString` object.

static let negativeSuffix: CFNumberFormatterKey!

Specifies the minus sign suffix symbol to use when placing a formatted number within a string, a `CFString` object.

static let paddingCharacter: CFNumberFormatterKey!

Specifies the padding character to use when placing a formatted number within a string, a `CFString` object.

static let paddingPosition: CFNumberFormatterKey!

Specifies the position of a formatted number within a string, a `CFNumber` object.

static let perMillSymbol: CFNumberFormatterKey!

Specifies the per mill (1/1000) symbol to use when placing a formatted number within a string, a `CFString` object.

static let percentSymbol: CFNumberFormatterKey!

Specifies the string that is used to represent the percent symbol, a `CFString` object.

static let plusSign: CFNumberFormatterKey!

Specifies the symbol for the plus sign, a `CFString` object.

static let positivePrefix: CFNumberFormatterKey!

Specifies the plus sign prefix symbol to use when placing a formatted number within a string, a `CFString` object.

static let positiveSuffix: CFNumberFormatterKey!

Specifies the plus sign suffix symbol to use when placing a formatted number within a string, a `CFString` object.

static let roundingIncrement: CFNumberFormatterKey!

Specifies a positive rounding increment, or `0.0` to disable rounding, a `CFNumber` object.

static let roundingMode: CFNumberFormatterKey!

Specifies how the last digit is rounded, as when `3.1415926535…` is rounded to three decimal places, as in `3.142`. See CFNumberFormatterRoundingMode for possible values.

static let secondaryGroupingSize: CFNumberFormatterKey!

Specifies how often the secondary grouping separator appears, a `CFNumber` object.

static let useGroupingSeparator: CFNumberFormatterKey!

Specifies if the grouping separator should be used, a `CFBoolean` object.

static let useSignificantDigits: CFNumberFormatterKey!

Specifies the whether the formatter uses significant digits, a `CFBoolean` object.

static let zeroSymbol: CFNumberFormatterKey!

Specifies the string that is used to represent zero, a `CFString` object.

static let minGroupingDigits: CFNumberFormatterKey!

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

struct CFLocaleKey

struct CFNotificationName

struct CFRunLoopMode

struct CFStreamPropertyKey

typealias CFTypeRef

An untyped “generic” reference to any Core Foundation object.

