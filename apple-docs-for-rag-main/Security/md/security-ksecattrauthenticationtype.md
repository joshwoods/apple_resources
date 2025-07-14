

- Security
-  kSecAttrAuthenticationType 

Global Variable

# kSecAttrAuthenticationType

A key whose value indicates the item’s authentication scheme.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrAuthenticationType: CFString
```

## Discussion

The corresponding value is of type CFString and denotes the authentication scheme for this item (see Authentication Type Values).

Note

For compatibility with earlier Keychain APIs, functions in Keychain services accept a CFNumber for the authentication scheme. The number is a 32-bit integer that encodes the authentication scheme as a `FourCharCode`. In your code, use a CFString with one of the values from Authentication Type Values instead of a number.

