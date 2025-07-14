

- Core Foundation
-  CFCharacterSetCreateBitmapRepresentation(\_:\_:) 

Function

# CFCharacterSetCreateBitmapRepresentation(\_:\_:)

Creates a new immutable data with the bitmap representation from the given character set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetCreateBitmapRepresentation(
    _ alloc: CFAllocator!,
    _ theSet: CFCharacterSet!
) -> CFData!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theSet`  

The set from which to create a bitmap representation. Refer to the comments for CFCharacterSetCreateWithBitmapRepresentation(_:_:) for the detailed discussion of the bitmap representation format.

## Return Value

A new CFData object containing a bitmap representation of `theSet`. Ownership follows the The Create Rule.

## See Also

### Querying Character Sets

func CFCharacterSetHasMemberInPlane(CFCharacterSet!, CFIndex) -> Bool

Reports whether or not a character set contains at least one member character in the specified plane.

func CFCharacterSetIsCharacterMember(CFCharacterSet!, UniChar) -> Bool

Reports whether or not a given Unicode character is in a character set.

func CFCharacterSetIsLongCharacterMember(CFCharacterSet!, UTF32Char) -> Bool

Reports whether or not a given UTF-32 character is in a character set.

func CFCharacterSetIsSupersetOfSet(CFCharacterSet!, CFCharacterSet!) -> Bool

Reports whether or not a character set is a superset of another set.

