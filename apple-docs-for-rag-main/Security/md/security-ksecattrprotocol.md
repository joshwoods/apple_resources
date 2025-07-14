

- Security
-  kSecAttrProtocol 

Global Variable

# kSecAttrProtocol

A key whose value indicates the item’s protocol.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrProtocol: CFString
```

## Mentioned in 

Adding a password to the keychain

## Discussion

The corresponding value is of type CFString and denotes the protocol for this item (see Protocol Values). Items of class kSecClassInternetPassword have this attribute.

Note

For compatibility with earlier Keychain APIs, functions in Keychain services accept a CFNumber for the protocol. The number is a 32-bit integer that encodes the protocol value as a `FourCharCode`. In your code, use a CFString with one of the values from Protocol Values instead of a number.

