

- Security
-  SecItemClass 

Enumeration

# SecItemClass

Specifies a keychain item’s class code.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SecItemClass
```

## Overview

These enumerations define constants your application can use to specify the type of the keychain item you wish to create, dispose, add, delete, update, copy, or locate. You can also use these constants with the tag constant SecItemAttr.

## Topics

### Constants

case internetPasswordItemClass

Indicates that the item is an Internet password.

case genericPasswordItemClass

Indicates that the item is a generic password.

case certificateItemClass

Indicates that the item is an X509 certificate.

case publicKeyItemClass

Indicates that the item is a public key of a public-private pair.

case privateKeyItemClass

Indicates that the item is a private key of a public-private pair.

case symmetricKeyItemClass

Indicates that the item is a private key used for symmetric-key encryption.

### Initializers

init?(rawValue: FourCharCode)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

