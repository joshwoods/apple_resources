

- Security
-  kSecAttrIsPermanent 

Global Variable

# kSecAttrIsPermanent

A key whose value indicates the item’s permanence.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrIsPermanent: CFString
```

## Mentioned in 

Generating New Cryptographic Keys

## Discussion

The corresponding value is of type CFBoolean and indicates whether or not this cryptographic key or key pair should be stored in the default keychain at creation time.

On key creation, if not explicitly specified, this attribute defaults to kCFBooleanFalse.

