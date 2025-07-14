

- Core Foundation
-  CFCharacterSetCreateWithCharactersInString(\_:\_:) 

Function

# CFCharacterSetCreateWithCharactersInString(\_:\_:)

Creates a new character set with the values in the given string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetCreateWithCharactersInString(
    _ alloc: CFAllocator!,
    _ theString: CFString!
) -> CFCharacterSet!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theString`  

A string containing the characters for the new set.

## Return Value

A new character set containing the characters from `theString`. Ownership follows the The Create Rule.

## See Also

### Creating Character Sets

func CFCharacterSetCreateCopy(CFAllocator!, CFCharacterSet!) -> CFCharacterSet!

Creates a new character set with the values from a given character set.

func CFCharacterSetCreateInvertedSet(CFAllocator!, CFCharacterSet!) -> CFCharacterSet!

Creates a new immutable character set that is the invert of the specified character set.

func CFCharacterSetCreateWithCharactersInRange(CFAllocator!, CFRange) -> CFCharacterSet!

Creates a new character set with the values from the given range of Unicode characters.

func CFCharacterSetCreateWithBitmapRepresentation(CFAllocator!, CFData!) -> CFCharacterSet!

Creates a new immutable character set with the bitmap representation specified by given data.

