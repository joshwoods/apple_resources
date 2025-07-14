

- Security
-  kSecCodeInfoSource 

Global Variable

# kSecCodeInfoSource

The source of the code signature used for the code object in a format suitable for display.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoSource: CFString
```

## Discussion

The value is a CFString object. This string is for display purposes only. Don’t rely on the precise value returned.

This is generic information returned regardless of which Code Signing Information Flags you pass to the SecCodeCopySigningInformation(_:_:_:) function.

