

- Security
-  kSecClassKey 

Global Variable

# kSecClassKey

The value that indicates a cryptographic key item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecClassKey: CFString
```

## Mentioned in 

Storing Keys in the Keychain

## Discussion

The following keychain item attributes form the composite primary key of a cryptographic key item:

- kSecAttrAccessGroup (on macOS, this key only applies if you set kSecUseDataProtectionKeychain or kSecAttrSynchronizable to true)

- kSecAttrApplicationLabel

- kSecAttrApplicationTag

- kSecAttrEffectiveKeySize

- kSecAttrKeyClass

- kSecAttrKeySizeInBits

- kSecAttrKeyType

- kSecAttrSynchronizable (on iOS 14 and newer, iOS 11 newer, and watchOS 7 and newer)

Calls to SecItemAdd(_:_:) that add a cryptographic key item with the same values for all of these attributes as an existing item result in errSecDuplicateItem.

The following keychain item attributes apply to a cryptographic key item, and don’t form part of its composite primary key:

- kSecAttrAccess (macOS only)

- kSecAttrAccessible (on macOS, this key only applies if you set kSecUseDataProtectionKeychain or kSecAttrSynchronizable to true)

- kSecAttrLabel

- kSecAttrIsPermanent

- kSecAttrPRF

- kSecAttrSalt

- kSecAttrRounds

- kSecAttrCanEncrypt

- kSecAttrCanDecrypt

- kSecAttrCanDerive

- kSecAttrCanSign

- kSecAttrCanVerify

- kSecAttrCanWrap

- kSecAttrCanUnwrap

