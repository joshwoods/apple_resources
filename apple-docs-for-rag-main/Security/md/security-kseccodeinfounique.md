

- Security
-  kSecCodeInfoUnique 

Global Variable

# kSecCodeInfoUnique

A key whose value is a binary number that uniquely identifies static code.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoUnique: CFString
```

## Discussion

The value is a CFData object. This identifier can be used to recognize this specific code in the future. This identifier is tied to the current version of the code, unlike the kSecCodeInfoIdentifier identifier, which remains stable across developer-approved updates. The algorithm used for the kSecCodeInfoUnique identifier may change over time. However, the identifier remains stable for existing, signed code.

This is generic information returned regardless of which Code Signing Information Flags you pass to the SecCodeCopySigningInformation(_:_:_:) function.

