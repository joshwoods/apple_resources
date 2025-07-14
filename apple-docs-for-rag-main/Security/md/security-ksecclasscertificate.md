

- Security
-  kSecClassCertificate 

Global Variable

# kSecClassCertificate

The value that indicates a certificate item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecClassCertificate: CFString
```

## Mentioned in 

Storing a Certificate in the Keychain

Storing an Identity in the Keychain

## Discussion

The following keychain item attributes form the composite primary key of a certificate password item:

- kSecAttrAccessGroup (on macOS, this key only applies if you set kSecUseDataProtectionKeychain or kSecAttrSynchronizable to true)

- kSecAttrCertificateType

- kSecAttrIssuer

- kSecAttrSerialNumber

- kSecAttrSynchronizable (on iOS 14 and newer, iOS 11 newer, and watchOS 7 and newer)

Calls to SecItemAdd(_:_:) that add a certificate item with the same values for all of these attributes as an existing item result in errSecDuplicateItem.

The following keychain item attributes apply to a certificate item, and don’t form part of its composite primary key:

- kSecAttrAccess (macOS only)

- kSecAttrAccessible (on macOS, this key only applies if you set kSecUseDataProtectionKeychain or kSecAttrSynchronizable to true)

- kSecAttrCertificateEncoding

- kSecAttrLabel

- kSecAttrSubject

- kSecAttrSubjectKeyID

- kSecAttrPublicKeyHash

