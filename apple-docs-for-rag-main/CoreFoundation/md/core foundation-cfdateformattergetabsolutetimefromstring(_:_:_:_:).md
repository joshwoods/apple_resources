

- Core Foundation
-  CFDateFormatterGetAbsoluteTimeFromString(\_:\_:\_:\_:) 

Function

# CFDateFormatterGetAbsoluteTimeFromString(\_:\_:\_:\_:)

Returns an absolute time object representing a given string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateFormatterGetAbsoluteTimeFromString(
    _ formatter: CFDateFormatter!,
    _ string: CFString!,
    _ rangep: UnsafeMutablePointer!,
    _ atp: UnsafeMutablePointer!
) -> Bool
```

## Parameters 

`formatter`  

The date formatter object to use to parse `string`.

`string`  

The string that contains the time to be parsed.

`rangep`  

Reference to the range within the string specifying the substring to be parsed. If `NULL`, the whole string is parsed. On return, the range that defines the extent of the parse (may be less than the given range).

`atp`  

An absolute time value, returned by reference, that represents `string`. Ownership follows the The Get Rule.

## Return Value

`true` if the string was parsed successfully, otherwise `false`.

## See Also

### Parsing Strings

func CFDateFormatterCreateDateFromString(CFAllocator!, CFDateFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!) -> CFDate!

Returns a date object representing a given string.

