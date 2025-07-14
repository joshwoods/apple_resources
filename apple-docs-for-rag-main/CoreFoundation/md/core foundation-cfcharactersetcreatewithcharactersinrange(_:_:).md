

- Core Foundation
-  CFCharacterSetCreateWithCharactersInRange(\_:\_:) 

Function

# CFCharacterSetCreateWithCharactersInRange(\_:\_:)

Creates a new character set with the values from the given range of Unicode characters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetCreateWithCharactersInRange(
    _ alloc: CFAllocator!,
    _ theRange: CFRange
) -> CFCharacterSet!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theRange`  

The Unicode range of characters of the new character set. The function accepts the range in 32-bit in the UTF-32 format. The valid character point range is from 0x00000 to 0x10FFFF.

## Return Value

A new character set that contains a contiguous range of Unicode characters. Ownership follows the The Create Rule.

## See Also

### Creating Character Sets

func CFCharacterSetCreateCopy(CFAllocator!, CFCharacterSet!) -> CFCharacterSet!

Creates a new character set with the values from a given character set.

func CFCharacterSetCreateInvertedSet(CFAllocator!, CFCharacterSet!) -> CFCharacterSet!

Creates a new immutable character set that is the invert of the specified character set.

func CFCharacterSetCreateWithCharactersInString(CFAllocator!, CFString!) -> CFCharacterSet!

Creates a new character set with the values in the given string.

func CFCharacterSetCreateWithBitmapRepresentation(CFAllocator!, CFData!) -> CFCharacterSet!

Creates a new immutable character set with the bitmap representation specified by given data.

