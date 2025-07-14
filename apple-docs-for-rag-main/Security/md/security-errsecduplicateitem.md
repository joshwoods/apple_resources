

- Security
-  errSecDuplicateItem 

Global Variable

# errSecDuplicateItem

The item already exists.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var errSecDuplicateItem: OSStatus { get }
```

## Discussion

The system considers an item to be a duplicate for a given keychain when that keychain already has an item of the same class with the same set of composite primary keys. Each class of keychain item has a different set of primary keys, although a few attributes are used in common across all classes. In particular, where applicable, kSecAttrSynchronizable and kSecAttrAccessGroup are part of the set of primary keys. The additional per-class primary keys are listed below:

For generic passwords, the primary keys include kSecAttrAccount and kSecAttrService.

For internet passwords, the primary keys include kSecAttrAccount, kSecAttrSecurityDomain, kSecAttrServer, kSecAttrProtocol, kSecAttrAuthenticationType, kSecAttrPort, and kSecAttrPath.

For certificates, the primary keys include kSecAttrCertificateType, kSecAttrIssuer, and kSecAttrSerialNumber.

For key items, the primary keys include kSecAttrKeyClass, kSecAttrKeyType, kSecAttrApplicationLabel, kSecAttrApplicationTag, kSecAttrKeySizeInBits, and kSecAttrEffectiveKeySize.

For identity items, which are a certificate and a private key bundled together, the primary keys are the same as for a certificate. Because a private key may be certified more than once, the uniqueness of the certificate determines that of the identity.

