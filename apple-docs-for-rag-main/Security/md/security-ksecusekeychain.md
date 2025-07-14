

- Security
-  kSecUseKeychain 

Global Variable

# kSecUseKeychain

A key whose value is a keychain to operate on.

macOS 10.7+

``` source
let kSecUseKeychain: CFString
```

## Discussion

Specifies a SecKeychain object that references the keychain to which SecItemAdd(_:_:) should add the provided items.

