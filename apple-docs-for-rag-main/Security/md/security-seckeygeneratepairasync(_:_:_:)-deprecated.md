

- Security
-  SecKeyGeneratePairAsync(\_:\_:\_:) Deprecated

Function

# SecKeyGeneratePairAsync(\_:\_:\_:)

Generates a public/private key pair.

macOS 10.7–12.0Deprecated

``` source
func SecKeyGeneratePairAsync(
    _ parameters: CFDictionary,
    _ deliveryQueue: dispatch_queue_t,
    _ result: @escaping SecKeyGeneratePairBlock
)
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

`deliveryQueue`  

The dispatch queue on which the result block should be scheduled.

`result`  

A block of type SecKeyGeneratePairBlock that gets called with the result upon completion.

