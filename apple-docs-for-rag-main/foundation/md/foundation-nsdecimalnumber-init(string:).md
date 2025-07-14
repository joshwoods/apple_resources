

- Foundation
- NSDecimalNumber
-  init(string:) 

Initializer

# init(string:)

Initializes a decimal number so that its value is equivalent to that in a given numeric string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(string numberValue: String?)
```

## Parameters 

`numberValue`  

A numeric string.

Besides digits, `numberValue` can include an initial `+` or `–`; a single `E` or `e`, to indicate the exponent of a number in scientific notation; and a single decimal separator character to divide the fractional from the integral part of the number. For a listing of acceptable and unacceptable strings, see init(string:locale:).

## Discussion

Don’t use this initializer if `numberValue` has a fractional part, since the lack of a locale makes handling the decimal separator ambiguous. The separator is a period in some locales (like in the United States) and a comma in others (such as France).

To parse a numeric string with a fractional part, use init(string:locale:) instead. When working with numeric representations with a known format, pass a fixed locale to ensure consistent results independent of the user’s current device settings. For localized parsing that uses the user’s current device settings, pass current.

## See Also

### Initializing a Decimal Number

init(decimal: Decimal)

Initializes a decimal number to represent a given decimal.

convenience init(mantissa: UInt64, exponent: Int16, isNegative: Bool)

Initializes a decimal number using the given mantissa, exponent, and sign.

convenience init(string: String?, locale: Any?)

Initializes a decimal number so that its value is equivalent to that in a given numeric string, interpreted using a given locale.

