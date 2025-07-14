

- Core Foundation
-  CFCharacterSetAddCharactersInString(\_:\_:) 

Function

# CFCharacterSetAddCharactersInString(\_:\_:)

Adds the characters in a given string to a character set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetAddCharactersInString(
    _ theSet: CFMutableCharacterSet!,
    _ theString: CFString!
)
```

## Parameters 

`theSet`  

The character set to modify.

`theString`  

A string containing the characters to add to `theSet`.

## See Also

### Adding Characters

func CFCharacterSetAddCharactersInRange(CFMutableCharacterSet!, CFRange)

Adds a given range to a character set.

