

- Security
-  kSecClassGenericPassword 

Global Variable

# kSecClassGenericPassword

The value that indicates a generic password item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecClassGenericPassword: CFString
```

## Mentioned in 

Adding a password to the keychain

## Discussion

The following keychain item attributes form the composite primary key of a generic password item:

- kSecAttrAccessGroup (on macOS, this key only applies if you set kSecUseDataProtectionKeychain or kSecAttrSynchronizable to true)

- kSecAttrAccount

- kSecAttrService

- kSecAttrSynchronizable

Calls to SecItemAdd(_:_:) that add a generic password item with the same values for all of these attributes as an existing item result in errSecDuplicateItem.

The following keychain item attributes apply to a generic password item, and don’t form part of its composite primary key:

- kSecAttrAccess (macOS only)

- kSecAttrAccessControl

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

- kSecAttrGeneric

