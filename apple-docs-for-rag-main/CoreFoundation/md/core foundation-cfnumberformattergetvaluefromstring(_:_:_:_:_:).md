

- Core Foundation
-  CFNumberFormatterGetValueFromString(\_:\_:\_:\_:\_:) 

Function

# CFNumberFormatterGetValueFromString(\_:\_:\_:\_:\_:)

Returns a number or value representing a given string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberFormatterGetValueFromString(
    _ formatter: CFNumberFormatter!,
    _ string: CFString!,
    _ rangep: UnsafeMutablePointer!,
    _ numberType: CFNumberType,
    _ valuePtr: UnsafeMutableRawPointer!
) -> Bool
```

## Parameters 

`formatter`  

The number formatter to use.

`string`  

The string to parse.

`rangep`  

A reference to a range that specifies the substring of `string` to be parsed. If `NULL`, the whole string is parsed. Upon return, contains the range of the actual extent of the parse (may be less than the given range).

`numberType`  

The type of value that `valuePtr` references. Valid values are listed in CFNumberType.

`valuePtr`  

Upon return, contains a number or value representing the string in the specified format. You are responsible for releasing this value.

## Return Value

`true` if the string was parsed successfully, otherwise `false`.

## See Also

### Formatting Values

func CFNumberFormatterCreateNumberFromString(CFAllocator!, CFNumberFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!, CFOptionFlags) -> CFNumber!

Returns a number object representing a given string.

func CFNumberFormatterCreateStringWithNumber(CFAllocator!, CFNumberFormatter!, CFNumber!) -> CFString!

Returns a string representation of the given number using the specified number formatter.

func CFNumberFormatterCreateStringWithValue(CFAllocator!, CFNumberFormatter!, CFNumberType, UnsafeRawPointer!) -> CFString!

Returns a string representation of the given number or value using the specified number formatter.

func CFNumberFormatterGetDecimalInfoForCurrencyCode(CFString!, UnsafeMutablePointer&lt;Int32>!, UnsafeMutablePointer&lt;Double>!) -> Bool

Returns the number of fraction digits that should be displayed, and the rounding increment, for a given currency.

