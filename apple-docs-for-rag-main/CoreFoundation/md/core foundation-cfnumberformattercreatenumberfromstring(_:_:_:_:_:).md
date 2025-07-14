

- Core Foundation
-  CFNumberFormatterCreateNumberFromString(\_:\_:\_:\_:\_:) 

Function

# CFNumberFormatterCreateNumberFromString(\_:\_:\_:\_:\_:)

Returns a number object representing a given string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberFormatterCreateNumberFromString(
    _ allocator: CFAllocator!,
    _ formatter: CFNumberFormatter!,
    _ string: CFString!,
    _ rangep: UnsafeMutablePointer!,
    _ options: CFOptionFlags
) -> CFNumber!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`formatter`  

The number formatter to use.

`string`  

The string to parse.

`rangep`  

A reference to a range that specifies the substring of `string` to be parsed. If `NULL`, the whole string is parsed. On return, contains the range of the actual extent of the parse (may be less than the given range).

`options`  

Specifies various configuration options to change the behavior of the parse. Currently, parseIntegersOnly is the only possible value for this parameter.

## Return Value

A new number that represents the given string. Returns `NULL` if there was a problem creating the number. Ownership follows the The Create Rule.

## See Also

### Formatting Values

func CFNumberFormatterCreateStringWithNumber(CFAllocator!, CFNumberFormatter!, CFNumber!) -> CFString!

Returns a string representation of the given number using the specified number formatter.

func CFNumberFormatterCreateStringWithValue(CFAllocator!, CFNumberFormatter!, CFNumberType, UnsafeRawPointer!) -> CFString!

Returns a string representation of the given number or value using the specified number formatter.

func CFNumberFormatterGetDecimalInfoForCurrencyCode(CFString!, UnsafeMutablePointer&lt;Int32>!, UnsafeMutablePointer&lt;Double>!) -> Bool

Returns the number of fraction digits that should be displayed, and the rounding increment, for a given currency.

func CFNumberFormatterGetValueFromString(CFNumberFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!, CFNumberType, UnsafeMutableRawPointer!) -> Bool

Returns a number or value representing a given string.

