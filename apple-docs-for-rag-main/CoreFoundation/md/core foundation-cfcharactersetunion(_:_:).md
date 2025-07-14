

- Core Foundation
-  CFCharacterSetUnion(\_:\_:) 

Function

# CFCharacterSetUnion(\_:\_:)

Forms the union of two character sets.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetUnion(
    _ theSet: CFMutableCharacterSet!,
    _ theOtherSet: CFCharacterSet!
)
```

## Parameters 

`theSet`  

The source character set, modified by union with `theOtherSet`.

`theOtherSet`  

The character set with which the union is formed.

## See Also

### Logical Operations

func CFCharacterSetIntersect(CFMutableCharacterSet!, CFCharacterSet!)

Forms an intersection of two character sets.

func CFCharacterSetInvert(CFMutableCharacterSet!)

Inverts the content of a given character set.

