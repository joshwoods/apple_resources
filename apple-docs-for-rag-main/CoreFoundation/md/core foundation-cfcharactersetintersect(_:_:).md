

- Core Foundation
-  CFCharacterSetIntersect(\_:\_:) 

Function

# CFCharacterSetIntersect(\_:\_:)

Forms an intersection of two character sets.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetIntersect(
    _ theSet: CFMutableCharacterSet!,
    _ theOtherSet: CFCharacterSet!
)
```

## Parameters 

`theSet`  

The source character set, modified by intersection with `theOtherSet`.

`theOtherSet`  

The character set with which the intersection is formed.

## See Also

### Logical Operations

func CFCharacterSetInvert(CFMutableCharacterSet!)

Inverts the content of a given character set.

func CFCharacterSetUnion(CFMutableCharacterSet!, CFCharacterSet!)

Forms the union of two character sets.

