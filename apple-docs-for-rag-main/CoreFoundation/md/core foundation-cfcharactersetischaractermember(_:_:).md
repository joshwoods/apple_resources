

- Core Foundation
-  CFCharacterSetIsCharacterMember(\_:\_:) 

Function

# CFCharacterSetIsCharacterMember(\_:\_:)

Reports whether or not a given Unicode character is in a character set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetIsCharacterMember(
    _ theSet: CFCharacterSet!,
    _ theChar: UniChar
) -> Bool
```

## Parameters 

`theSet`  

The character set to examine.

`theChar`  

The Unicode character for which to test against the character set. Note that this function takes 16-bit Unicode character value; hence, it does not support access to the non-BMP planes.

## Return Value

`true` if `theSet` contains `theChar`, otherwise `false`.

## See Also

### Querying Character Sets

func CFCharacterSetCreateBitmapRepresentation(CFAllocator!, CFCharacterSet!) -> CFData!

Creates a new immutable data with the bitmap representation from the given character set.

func CFCharacterSetHasMemberInPlane(CFCharacterSet!, CFIndex) -> Bool

Reports whether or not a character set contains at least one member character in the specified plane.

func CFCharacterSetIsLongCharacterMember(CFCharacterSet!, UTF32Char) -> Bool

Reports whether or not a given UTF-32 character is in a character set.

func CFCharacterSetIsSupersetOfSet(CFCharacterSet!, CFCharacterSet!) -> Bool

Reports whether or not a character set is a superset of another set.

