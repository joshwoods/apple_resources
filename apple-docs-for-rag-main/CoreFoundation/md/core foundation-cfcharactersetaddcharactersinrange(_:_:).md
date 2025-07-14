

- Core Foundation
-  CFCharacterSetAddCharactersInRange(\_:\_:) 

Function

# CFCharacterSetAddCharactersInRange(\_:\_:)

Adds a given range to a character set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetAddCharactersInRange(
    _ theSet: CFMutableCharacterSet!,
    _ theRange: CFRange
)
```

## Parameters 

`theSet`  

The character set to modify.

`theRange`  

The range to add to the character set. The range is specified in 32-bits in UTF-32 format, and must lie within the valid Unicode character range (from `0x00000` to `0x10FFFF`).

## See Also

### Adding Characters

func CFCharacterSetAddCharactersInString(CFMutableCharacterSet!, CFString!)

Adds the characters in a given string to a character set.

