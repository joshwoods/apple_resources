

- Core Foundation
-  CFCharacterSetIsLongCharacterMember(\_:\_:) 

Function

# CFCharacterSetIsLongCharacterMember(\_:\_:)

Reports whether or not a given UTF-32 character is in a character set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetIsLongCharacterMember(
    _ theSet: CFCharacterSet!,
    _ theChar: UTF32Char
) -> Bool
```

## Parameters 

`theSet`  

The character set to examine.

`theChar`  

The UTF-32 character for which to test against the character set.

## Return Value

`true` if `theSet` contains `theChar`, otherwise `false`.

## See Also

### Querying Character Sets

func CFCharacterSetCreateBitmapRepresentation(CFAllocator!, CFCharacterSet!) -> CFData!

Creates a new immutable data with the bitmap representation from the given character set.

func CFCharacterSetHasMemberInPlane(CFCharacterSet!, CFIndex) -> Bool

Reports whether or not a character set contains at least one member character in the specified plane.

func CFCharacterSetIsCharacterMember(CFCharacterSet!, UniChar) -> Bool

Reports whether or not a given Unicode character is in a character set.

func CFCharacterSetIsSupersetOfSet(CFCharacterSet!, CFCharacterSet!) -> Bool

Reports whether or not a character set is a superset of another set.

