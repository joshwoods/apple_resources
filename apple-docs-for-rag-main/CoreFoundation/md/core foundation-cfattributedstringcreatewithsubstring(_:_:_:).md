

- Core Foundation
-  CFAttributedStringCreateWithSubstring(\_:\_:\_:) 

Function

# CFAttributedStringCreateWithSubstring(\_:\_:\_:)

Creates a sub-attributed string from the specified range.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringCreateWithSubstring(
    _ alloc: CFAllocator!,
    _ aStr: CFAttributedString!,
    _ range: CFRange
) -> CFAttributedString!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new attributed string. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`aStr`  

The attributed string to copy.

`range`  

The range of the attributed string to copy. `range` must not exceed the bounds of `aStr`.

## Return Value

A new attributed string whose string and attributes are copied from the specified range of the supplied attributed string. Returns `NULL` if there was a problem copying the object. Ownership follows the The Create Rule.

## See Also

### Creating a CFAttributedString

func CFAttributedStringCreate(CFAllocator!, CFString!, CFDictionary!) -> CFAttributedString!

Creates an attributed string with specified string and attributes.

func CFAttributedStringCreateCopy(CFAllocator!, CFAttributedString!) -> CFAttributedString!

Creates an immutable copy of an attributed string.

func CFAttributedStringGetLength(CFAttributedString!) -> CFIndex

Returns the length of the attributed string in characters.

func CFAttributedStringGetString(CFAttributedString!) -> CFString!

Returns the string for an attributed string.

