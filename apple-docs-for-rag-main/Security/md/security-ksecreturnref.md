

- Security
-  kSecReturnRef 

Global Variable

# kSecReturnRef

A key whose value is a Boolean indicating whether or not to return a reference to an item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecReturnRef: CFString
```

## Mentioned in 

Storing a Certificate in the Keychain

## Discussion

The corresponding value is of type CFBoolean. A value of kCFBooleanTrue indicates that a reference should be returned. Depending on the item class requested, the returned references may be of type SecKeychainItem, SecKey, SecCertificate, SecIdentity, or CFData.

