

- Security
-  kSecValueRef 

Global Variable

# kSecValueRef

A key whose value is a reference to the item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecValueRef: CFString
```

## Discussion

The corresponding value, depending on the item class requested, is of type SecKeychainItem, SecKey, SecCertificate, or SecIdentity.

