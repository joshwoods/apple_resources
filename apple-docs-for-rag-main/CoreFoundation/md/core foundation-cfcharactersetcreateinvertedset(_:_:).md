

- Core Foundation
-  CFCharacterSetCreateInvertedSet(\_:\_:) 

Function

# CFCharacterSetCreateInvertedSet(\_:\_:)

Creates a new immutable character set that is the invert of the specified character set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetCreateInvertedSet(
    _ alloc: CFAllocator!,
    _ theSet: CFCharacterSet!
) -> CFCharacterSet!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theSet`  

The character set from which to create an inverted set.

## Return Value

A new character set that is the invert of `theSet`. Ownership follows the The Create Rule.

## See Also

### Creating Character Sets

func CFCharacterSetCreateCopy(CFAllocator!, CFCharacterSet!) -> CFCharacterSet!

Creates a new character set with the values from a given character set.

func CFCharacterSetCreateWithCharactersInRange(CFAllocator!, CFRange) -> CFCharacterSet!

Creates a new character set with the values from the given range of Unicode characters.

func CFCharacterSetCreateWithCharactersInString(CFAllocator!, CFString!) -> CFCharacterSet!

Creates a new character set with the values in the given string.

func CFCharacterSetCreateWithBitmapRepresentation(CFAllocator!, CFData!) -> CFCharacterSet!

Creates a new immutable character set with the bitmap representation specified by given data.

