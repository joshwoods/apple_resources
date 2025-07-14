

- Core Foundation
- CFNumberFormatterKey
-  roundingMode 

Type Property

# roundingMode

Specifies how the last digit is rounded, as when `3.1415926535…` is rounded to three decimal places, as in `3.142`. See CFNumberFormatterRoundingMode for possible values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let roundingMode: CFNumberFormatterKey!
```

## See Also

### Constants

static let currencyCode: CFNumberFormatterKey!

Specifies the currency code, a `CFString` object.

static let decimalSeparator: CFNumberFormatterKey!

Specifies the decimal separator, a `CFString` object.

static let currencyDecimalSeparator: CFNumberFormatterKey!

Specifies the currency decimal separator, a `CFString` object.

static let alwaysShowDecimalSeparator: CFNumberFormatterKey!

Specifies if the result of converting a value to a string should always contain the decimal separator, even if the number is an integer.

static let groupingSeparator: CFNumberFormatterKey!

Specifies the grouping separator, a `CFString` object.

static let useGroupingSeparator: CFNumberFormatterKey!

Specifies if the grouping separator should be used, a `CFBoolean` object.

static let percentSymbol: CFNumberFormatterKey!

Specifies the string that is used to represent the percent symbol, a `CFString` object.

static let zeroSymbol: CFNumberFormatterKey!

Specifies the string that is used to represent zero, a `CFString` object.

static let naNSymbol: CFNumberFormatterKey!

Specifies the string that is used to represent NaN (“not a number”) when values are converted to strings, a `CFString` object.

static let infinitySymbol: CFNumberFormatterKey!

Specifies the string that is used to represent the symbol for infinity, a `CFString` object.

static let minusSign: CFNumberFormatterKey!

Specifies the symbol for the minus sign, a `CFString` object.

static let plusSign: CFNumberFormatterKey!

Specifies the symbol for the plus sign, a `CFString` object.

static let currencySymbol: CFNumberFormatterKey!

Specifies the symbol for the currency, a `CFString` object.

static let exponentSymbol: CFNumberFormatterKey!

Specifies the exponent symbol (“E” or “e”) in the scientific notation of numbers (for example, as in `1.0e+56`), a `CFString` object.

static let minIntegerDigits: CFNumberFormatterKey!

Specifies the minimum number of integer digits before a decimal point, a `CFNumber` object.

