

- Core Foundation
-  CFCharacterSetIsSupersetOfSet(\_:\_:) 

Function

# CFCharacterSetIsSupersetOfSet(\_:\_:)

Reports whether or not a character set is a superset of another set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetIsSupersetOfSet(
    _ theSet: CFCharacterSet!,
    _ theOtherset: CFCharacterSet!
) -> Bool
```

## Parameters 

`theSet`  

The character set to be checked for the membership of `theOtherSet`.

`theOtherset`  

The character set to be checked whether or not it is a subset of `theSet`.

## Return Value

`true` if `theSet` is a superset of `theOtherSet`, otherwise `false`.

## See Also

### Querying Character Sets

func CFCharacterSetCreateBitmapRepresentation(CFAllocator!, CFCharacterSet!) -> CFData!

Creates a new immutable data with the bitmap representation from the given character set.

func CFCharacterSetHasMemberInPlane(CFCharacterSet!, CFIndex) -> Bool

Reports whether or not a character set contains at least one member character in the specified plane.

func CFCharacterSetIsCharacterMember(CFCharacterSet!, UniChar) -> Bool

Reports whether or not a given Unicode character is in a character set.

func CFCharacterSetIsLongCharacterMember(CFCharacterSet!, UTF32Char) -> Bool

Reports whether or not a given UTF-32 character is in a character set.

