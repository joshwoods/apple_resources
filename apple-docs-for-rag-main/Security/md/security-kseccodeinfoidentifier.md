

- Security
-  kSecCodeInfoIdentifier 

Global Variable

# kSecCodeInfoIdentifier

A key whose value is the signing identifier sealed into the signature.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoIdentifier: CFString
```

## Discussion

The value is a CFString object. Absent for unsigned code.

This is generic information returned regardless of which Code Signing Information Flags you pass to the SecCodeCopySigningInformation(_:_:_:) function.

