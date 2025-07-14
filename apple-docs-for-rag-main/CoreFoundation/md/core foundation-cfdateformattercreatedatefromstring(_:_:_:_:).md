

- Core Foundation
-  CFDateFormatterCreateDateFromString(\_:\_:\_:\_:) 

Function

# CFDateFormatterCreateDateFromString(\_:\_:\_:\_:)

Returns a date object representing a given string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateFormatterCreateDateFromString(
    _ allocator: CFAllocator!,
    _ formatter: CFDateFormatter!,
    _ string: CFString!,
    _ rangep: UnsafeMutablePointer!
) -> CFDate!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`formatter`  

The date formatter object to use to parse `string`.

`string`  

The string that contains the date.

`rangep`  

A reference to the range within the string specifying the substring to be parsed. If `NULL`, the whole string is parsed. Upon return, contains the range that defines the extent of the parse (may be less than the given range).

## Return Value

A new date that represents `string`, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### Parsing Strings

func CFDateFormatterGetAbsoluteTimeFromString(CFDateFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!, UnsafeMutablePointer&lt;CFAbsoluteTime>!) -> Bool

Returns an absolute time object representing a given string.

