

- Core Foundation
-  CFCharacterSetRemoveCharactersInString(\_:\_:) 

Function

# CFCharacterSetRemoveCharactersInString(\_:\_:)

Removes the characters in a given string from a character set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetRemoveCharactersInString(
    _ theSet: CFMutableCharacterSet!,
    _ theString: CFString!
)
```

## Parameters 

`theSet`  

The character set to modify.

`theString`  

A string containing the characters to remove from `theSet`.

## See Also

### Removing Characters

func CFCharacterSetRemoveCharactersInRange(CFMutableCharacterSet!, CFRange)

Removes a given range of Unicode characters from a character set.

