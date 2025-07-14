

- Security
-  kSecCodeInfoFormat 

Global Variable

# kSecCodeInfoFormat

A key whose value is a string representing the type and format of the code in a form suitable for display to a knowledgeable user.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoFormat: CFString
```

## Discussion

The value is a CFString object.

This is generic information returned regardless of which Code Signing Information Flags you pass to the SecCodeCopySigningInformation(_:_:_:) function.

