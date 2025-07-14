

- Security
-  kSecAttrCanSign 

Global Variable

# kSecAttrCanSign

A key whose value is a Boolean that indicates whether the cryptographic key can be used for digital signing.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrCanSign: CFString
```

## Mentioned in 

Signing and Verifying

## Discussion

The corresponding value is of type CFBoolean and indicates whether this cryptographic key can be used to create a digital signature.

On key creation, if not explicitly specified, this attribute defaults to kCFBooleanTrue for private keys and kCFBooleanFalse for public keys.

