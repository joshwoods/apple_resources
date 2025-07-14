

- Security
-  SecKeyGenerateSymmetric(\_:\_:) Deprecated

Function

# SecKeyGenerateSymmetric(\_:\_:)

Generates a random symmetric key.

macOS 10.7–12.0Deprecated

``` source
func SecKeyGenerateSymmetric(
    _ parameters: CFDictionary,
    _ error: UnsafeMutablePointer?>?
) -> SecKey?
```

Deprecated

No longer supported

## Parameters 

`parameters`  

A key generation parameter dictionary. At minimum, this must contain kSecAttrKeyType and kSecAttrKeySizeInBits. In addition, this function assumes default values for the following keys:

- kSecAttrLabel defaults to `NULL`.

- kSecAttrIsPermanent if this key is present and has a value of kCFBooleanTrue, the key or key pair will be added to the default keychain.

- kSecAttrApplicationTag defaults to `NULL`.

- kSecAttrEffectiveKeySize defaults to `NULL`, which means the effective key size is the same as the key size (kSecAttrKeySizeInBits).

- kSecAttrCanEncrypt defaults to kCFBooleanFalse for private keys, kCFBooleanTrue for public keys.

- kSecAttrCanDecrypt defaults to kCFBooleanTrue for private keys, kCFBooleanFalse for public keys.

- kSecAttrCanDerive defaults to kCFBooleanTrue.

- kSecAttrCanSign defaults to kCFBooleanTrue for private keys, kCFBooleanFalse for public keys.

- kSecAttrCanVerify defaults to kCFBooleanFalse for private keys, kCFBooleanTrue for public keys.

- kSecAttrCanWrap defaults to kCFBooleanFalse for private keys, kCFBooleanTrue for public keys.

- kSecAttrCanUnwrap defaults to kCFBooleanTrue for private keys, kCFBooleanFalse for public keys.

These default values can be overridden by adding a value for the associated key in the parameter dictionary.

When used as a replacement for SecKeyGenerate, set the kSecUseKeychain key to the keychain (SecKeychain) into which the key should be stored, kSecAttrLabel to a user-visible label for the key, and kSecAttrApplicationLabel to an identifier defined by your application, for subsequent use in calls to SecItemCopyMatching(_:_:). Additionally, you can specify keychain access controls for the key by setting kSecAttrAccess to a SecAccess object.

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 variable where an error object is stored upon failure. If not `NULL`, the caller is responsible for checking this variable and releasing the resulting object if it exists.

## Return Value

A newly generated symmetric key, or `NULL` on failure. In Objective-C, call the CFRelease function to free the key’s memory when you are done with it.

