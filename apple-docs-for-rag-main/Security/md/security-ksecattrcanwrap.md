

- Security
-  kSecAttrCanWrap 

Global Variable

# kSecAttrCanWrap

A key whose value is a Boolean that indicates whether the cryptographic key can be used for wrapping.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrCanWrap: CFString
```

## Discussion

The corresponding value is of type CFBoolean and indicates whether this cryptographic key can be used to wrap another key.

On key creation, if not explicitly specified, this attribute defaults to kCFBooleanFalse for private keys and kCFBooleanTrue for public keys.

