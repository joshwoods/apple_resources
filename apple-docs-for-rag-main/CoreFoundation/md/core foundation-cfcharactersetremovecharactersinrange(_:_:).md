

- Core Foundation
-  CFCharacterSetRemoveCharactersInRange(\_:\_:) 

Function

# CFCharacterSetRemoveCharactersInRange(\_:\_:)

Removes a given range of Unicode characters from a character set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetRemoveCharactersInRange(
    _ theSet: CFMutableCharacterSet!,
    _ theRange: CFRange
)
```

## Parameters 

`theSet`  

The character set to modify.

`theRange`  

The range to remove from the character set. The range is specified in 32-bits in UTF-32 format, and must lie within the valid Unicode character range (from `0x00000` to `0x10FFFF`).

## See Also

### Removing Characters

func CFCharacterSetRemoveCharactersInString(CFMutableCharacterSet!, CFString!)

Removes the characters in a given string from a character set.

