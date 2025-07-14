

- Core Foundation
-  CFCharacterSetCreateWithBitmapRepresentation(\_:\_:) 

Function

# CFCharacterSetCreateWithBitmapRepresentation(\_:\_:)

Creates a new immutable character set with the bitmap representation specified by given data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetCreateWithBitmapRepresentation(
    _ alloc: CFAllocator!,
    _ theData: CFData!
) -> CFCharacterSet!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theData`  

A CFData object that specifies the bitmap representation of the Unicode character points the for the new character set. The bitmap representation could contain all the Unicode character range starting from BMP to Plane 16. The first 8KiB (8192 bytes) of the data represent the BMP range. The BMP range 8KiB can be followed by zero to sixteen 8KiB bitmaps, each prepended with the plane index byte. For example, the bitmap representing the BMP and Plane 2 has the size of 16385 bytes (8KiB for BMP, 1 byte index, and a 8KiB bitmap for Plane 2). The plane index byte, in this case, contains the integer value two.

If the data contains a Plane index byte outside of the valid Plane range (1 to 16), the behavior is undefined.

## Return Value

A new character set containing the indicated characters from `theData`. Ownership follows the The Create Rule.

## See Also

### Creating Character Sets

func CFCharacterSetCreateCopy(CFAllocator!, CFCharacterSet!) -> CFCharacterSet!

Creates a new character set with the values from a given character set.

func CFCharacterSetCreateInvertedSet(CFAllocator!, CFCharacterSet!) -> CFCharacterSet!

Creates a new immutable character set that is the invert of the specified character set.

func CFCharacterSetCreateWithCharactersInRange(CFAllocator!, CFRange) -> CFCharacterSet!

Creates a new character set with the values from the given range of Unicode characters.

func CFCharacterSetCreateWithCharactersInString(CFAllocator!, CFString!) -> CFCharacterSet!

Creates a new character set with the values in the given string.

