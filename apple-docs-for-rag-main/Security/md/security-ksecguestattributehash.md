

- Security
-  kSecGuestAttributeHash 

Global Variable

# kSecGuestAttributeHash

A key whose value is a data object containing the SHA-1 hash of the code directory.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecGuestAttributeHash: CFString
```

## Discussion

This hash can be used as a unique identifier to recognize this specific code in the future. This identifier is tied to the current version of the code, unlike the kSecCodeInfoIdentifier identifier, which remains stable across developer-approved updates. If you are not passing this hash in the attribute dictionary when you call the SecHostCreateGuest function, then you must pass the kSecCSGenerateGuestHash flag to the function as well.

