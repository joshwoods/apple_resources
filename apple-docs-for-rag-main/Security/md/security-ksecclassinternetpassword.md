

- Security
-  kSecClassInternetPassword 

Global Variable

# kSecClassInternetPassword

The value that indicates an Internet password item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecClassInternetPassword: CFString
```

## Discussion

The following keychain item attributes form the composite primary key of an Internet password item:

- kSecAttrAccessGroup (on macOS, this key only applies if you set kSecUseDataProtectionKeychain or kSecAttrSynchronizable to true)

- kSecAttrAccount

- kSecAttrAuthenticationType

- kSecAttrPath

- kSecAttrPort

- kSecAttrProtocol

- kSecAttrSecurityDomain

- kSecAttrServer

- kSecAttrSynchronizable

Calls to SecItemAdd(_:_:) that add an Internet password item with the same values for all of these attributes as an existing item result in errSecDuplicateItem.

The following keychain item attributes apply to an Internet password item, and don’t form part of its composite primary key:

- kSecAttrAccess (macOS only)

- kSecAttrAccessible (on macOS, this key only applies if you set kSecUseDataProtectionKeychain or kSecAttrSynchronizable to true)

- kSecAttrCreationDate

- kSecAttrModificationDate

- kSecAttrDescription

- kSecAttrComment

- kSecAttrCreator

- kSecAttrType

- kSecAttrLabel

- kSecAttrIsInvisible

- kSecAttrIsNegative

