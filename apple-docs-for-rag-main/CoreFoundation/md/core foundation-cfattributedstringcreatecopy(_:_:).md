

- Core Foundation
-  CFAttributedStringCreateCopy(\_:\_:) 

Function

# CFAttributedStringCreateCopy(\_:\_:)

Creates an immutable copy of an attributed string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringCreateCopy(
    _ alloc: CFAllocator!,
    _ aStr: CFAttributedString!
) -> CFAttributedString!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new attributed string. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`aStr`  

The attributed string to copy.

## Return Value

An immutable attributed string with characters and attributes identical to those of `aStr`. Returns `NULL` if there was a problem copying the object. Ownership follows the The Create Rule.

## See Also

### Creating a CFAttributedString

func CFAttributedStringCreate(CFAllocator!, CFString!, CFDictionary!) -> CFAttributedString!

Creates an attributed string with specified string and attributes.

func CFAttributedStringCreateWithSubstring(CFAllocator!, CFAttributedString!, CFRange) -> CFAttributedString!

Creates a sub-attributed string from the specified range.

func CFAttributedStringGetLength(CFAttributedString!) -> CFIndex

Returns the length of the attributed string in characters.

func CFAttributedStringGetString(CFAttributedString!) -> CFString!

Returns the string for an attributed string.

