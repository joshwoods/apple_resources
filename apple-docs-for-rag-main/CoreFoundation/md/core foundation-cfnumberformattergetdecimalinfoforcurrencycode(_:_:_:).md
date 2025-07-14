

- Core Foundation
-  CFNumberFormatterGetDecimalInfoForCurrencyCode(\_:\_:\_:) 

Function

# CFNumberFormatterGetDecimalInfoForCurrencyCode(\_:\_:\_:)

Returns the number of fraction digits that should be displayed, and the rounding increment, for a given currency.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberFormatterGetDecimalInfoForCurrencyCode(
    _ currencyCode: CFString!,
    _ defaultFractionDigits: UnsafeMutablePointer!,
    _ roundingIncrement: UnsafeMutablePointer!
) -> Bool
```

## Parameters 

`currencyCode`  

A string containing a ISO 4217 3-letter currency code. For example, AUD for Australian Dollars, EUR for Euros.

`defaultFractionDigits`  

Upon return, contains the number of fraction digits that should be displayed for the currency specified by `currencyCode`.

`roundingIncrement`  

Upon return, contains the rounding increment for the currency specified by `currencyCode`, or `0.0` if no rounding is done by the currency.

## Return Value

`true` if the information was obtained successfully, otherwise `false` (for example, if the currency code is unknown or the information is not available).

## Discussion

The returned values are not localized because these are properties of the currency.

## See Also

### Formatting Values

func CFNumberFormatterCreateNumberFromString(CFAllocator!, CFNumberFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!, CFOptionFlags) -> CFNumber!

Returns a number object representing a given string.

func CFNumberFormatterCreateStringWithNumber(CFAllocator!, CFNumberFormatter!, CFNumber!) -> CFString!

Returns a string representation of the given number using the specified number formatter.

func CFNumberFormatterCreateStringWithValue(CFAllocator!, CFNumberFormatter!, CFNumberType, UnsafeRawPointer!) -> CFString!

Returns a string representation of the given number or value using the specified number formatter.

func CFNumberFormatterGetValueFromString(CFNumberFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!, CFNumberType, UnsafeMutableRawPointer!) -> Bool

Returns a number or value representing a given string.

