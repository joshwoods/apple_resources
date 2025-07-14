

- Security
-  kSecAttrTokenIDSecureEnclave 

Global Variable

# kSecAttrTokenIDSecureEnclave

Specifies an item should be stored in the device’s Secure Enclave.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrTokenIDSecureEnclave: CFString
```

## Mentioned in 

Protecting keys with the Secure Enclave

## Discussion

The only keychain items supported by the Secure Enclave are 256-bit elliptic curve private keys (those that have key type kSecAttrKeyTypeEC). Such keys must be generated directly on the Secure Enclave using the SecKeyGeneratePair(_:_:_:) function with the kSecAttrTokenID key set to kSecAttrTokenIDSecureEnclave in the parameters dictionary.

Important

It is not possible to import pre-existing keys into the Secure Enclave.

