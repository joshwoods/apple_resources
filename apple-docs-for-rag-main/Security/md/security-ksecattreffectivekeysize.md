

- Security
-  kSecAttrEffectiveKeySize 

Global Variable

# kSecAttrEffectiveKeySize

A key whose value indicates the effective number of bits in a cryptographic key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrEffectiveKeySize: CFString
```

## Discussion

The corresponding value is of type CFNumber and indicates the effective number of bits in this cryptographic key. For example, a DES key has a kSecAttrKeySizeInBits of 64, but a kSecAttrEffectiveKeySize of 56 bits.

