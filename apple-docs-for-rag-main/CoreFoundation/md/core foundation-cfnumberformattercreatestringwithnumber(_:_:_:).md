

- Core Foundation
-  CFNumberFormatterCreateStringWithNumber(\_:\_:\_:) 

Function

# CFNumberFormatterCreateStringWithNumber(\_:\_:\_:)

Returns a string representation of the given number using the specified number formatter.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberFormatterCreateStringWithNumber(
    _ allocator: CFAllocator!,
    _ formatter: CFNumberFormatter!,
    _ number: CFNumber!
) -> CFString!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`formatter`  

The number formatter to use.

`number`  

The number from which to create a string representation.

## Return Value

A new string that represents the given number in the specified format. Returns `NULL` if there was a problem creating the string. Ownership follows the The Create Rule.

## See Also

### Formatting Values

func CFNumberFormatterCreateNumberFromString(CFAllocator!, CFNumberFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!, CFOptionFlags) -> CFNumber!

Returns a number object representing a given string.

func CFNumberFormatterCreateStringWithValue(CFAllocator!, CFNumberFormatter!, CFNumberType, UnsafeRawPointer!) -> CFString!

Returns a string representation of the given number or value using the specified number formatter.

func CFNumberFormatterGetDecimalInfoForCurrencyCode(CFString!, UnsafeMutablePointer&lt;Int32>!, UnsafeMutablePointer&lt;Double>!) -> Bool

Returns the number of fraction digits that should be displayed, and the rounding increment, for a given currency.

func CFNumberFormatterGetValueFromString(CFNumberFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!, CFNumberType, UnsafeMutableRawPointer!) -> Bool

Returns a number or value representing a given string.

