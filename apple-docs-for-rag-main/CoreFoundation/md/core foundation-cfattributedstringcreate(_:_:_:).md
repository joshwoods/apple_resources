

- Core Foundation
-  CFAttributedStringCreate(\_:\_:\_:) 

Function

# CFAttributedStringCreate(\_:\_:\_:)

Creates an attributed string with specified string and attributes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringCreate(
    _ alloc: CFAllocator!,
    _ str: CFString!,
    _ attributes: CFDictionary!
) -> CFAttributedString!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new attributed string. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`str`  

A string that specifies the characters to use in the new attributed string. This value is copied.

`attributes`  

A dictionary that contains the attributes to apply to the new attributed string. This value is copied.

## Return Value

An attributed string that contains the characters from `str` and the attributes specified by `attributes`. The result is `NULL` if there was a problem in creating the attributed string. Ownership follows the The Create Rule.

## Discussion

Note that both the string and the attributes dictionary are copied. The specified attributes are applied to the whole string. If you want to apply different attributes to different ranges of the string, you should use a mutable attributed string.

## See Also

### Creating a CFAttributedString

func CFAttributedStringCreateCopy(CFAllocator!, CFAttributedString!) -> CFAttributedString!

Creates an immutable copy of an attributed string.

func CFAttributedStringCreateWithSubstring(CFAllocator!, CFAttributedString!, CFRange) -> CFAttributedString!

Creates a sub-attributed string from the specified range.

func CFAttributedStringGetLength(CFAttributedString!) -> CFIndex

Returns the length of the attributed string in characters.

func CFAttributedStringGetString(CFAttributedString!) -> CFString!

Returns the string for an attributed string.

