

- Core Foundation
-  CFNumberFormatterCreateStringWithValue(\_:\_:\_:\_:) 

Function

# CFNumberFormatterCreateStringWithValue(\_:\_:\_:\_:)

Returns a string representation of the given number or value using the specified number formatter.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberFormatterCreateStringWithValue(
    _ allocator: CFAllocator!,
    _ formatter: CFNumberFormatter!,
    _ numberType: CFNumberType,
    _ valuePtr: UnsafeRawPointer!
) -> CFString!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`formatter`  

The number formatter to use.

`numberType`  

The type of value that `valuePtr` references. Valid values are listed in CFNumberType.

`valuePtr`  

A pointer to the value to be converted.

## Return Value

A new string that represents the given number or value formatted by `formatter`. Returns `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### Formatting Values

func CFNumberFormatterCreateNumberFromString(CFAllocator!, CFNumberFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!, CFOptionFlags) -> CFNumber!

Returns a number object representing a given string.

func CFNumberFormatterCreateStringWithNumber(CFAllocator!, CFNumberFormatter!, CFNumber!) -> CFString!

Returns a string representation of the given number using the specified number formatter.

func CFNumberFormatterGetDecimalInfoForCurrencyCode(CFString!, UnsafeMutablePointer&lt;Int32>!, UnsafeMutablePointer&lt;Double>!) -> Bool

Returns the number of fraction digits that should be displayed, and the rounding increment, for a given currency.

func CFNumberFormatterGetValueFromString(CFNumberFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!, CFNumberType, UnsafeMutableRawPointer!) -> Bool

Returns a number or value representing a given string.

