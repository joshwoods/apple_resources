

- Core Foundation
-  CFCharacterSetHasMemberInPlane(\_:\_:) 

Function

# CFCharacterSetHasMemberInPlane(\_:\_:)

Reports whether or not a character set contains at least one member character in the specified plane.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetHasMemberInPlane(
    _ theSet: CFCharacterSet!,
    _ thePlane: CFIndex
) -> Bool
```

## Parameters 

`theSet`  

The character set to examine.

`thePlane`  

The plane number to be checked for the membership. The valid value range is from 0 to 16. If the value is outside of the valid plane number range, the behavior is undefined.

## Return Value

`true` if at least one member character is in the specified plane, otherwise `false`.

## See Also

### Querying Character Sets

func CFCharacterSetCreateBitmapRepresentation(CFAllocator!, CFCharacterSet!) -> CFData!

Creates a new immutable data with the bitmap representation from the given character set.

func CFCharacterSetIsCharacterMember(CFCharacterSet!, UniChar) -> Bool

Reports whether or not a given Unicode character is in a character set.

func CFCharacterSetIsLongCharacterMember(CFCharacterSet!, UTF32Char) -> Bool

Reports whether or not a given UTF-32 character is in a character set.

func CFCharacterSetIsSupersetOfSet(CFCharacterSet!, CFCharacterSet!) -> Bool

Reports whether or not a character set is a superset of another set.

