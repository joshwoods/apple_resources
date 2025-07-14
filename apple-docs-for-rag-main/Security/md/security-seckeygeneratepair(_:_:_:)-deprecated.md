

- Security
-  SecKeyGeneratePair(\_:\_:\_:) Deprecated

Function

# SecKeyGeneratePair(\_:\_:\_:)

Creates an asymmetric key pair.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.7–12.0DeprecatedtvOS 4.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–8.0Deprecated

``` source
func SecKeyGeneratePair(
    _ parameters: CFDictionary,
    _ publicKey: UnsafeMutablePointer?,
    _ privateKey: UnsafeMutablePointer?
) -> OSStatus
```

Deprecated

Use SecKeyCreateRandomKey

## Parameters 

`parameters`  

A dictionary of key-value pairs that specify the type of keys to be generated.

`publicKey`  

On return, points to the keychain item object of the new public key. In Objective-C, call the CFRelease function to release this object when you are finished with it.

`privateKey`  

On return, points to the keychain item object of the new private key. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

In order to generate a key pair, the dictionary passed in the `parameters` parameter must contain at least the following key-value pairs:

- A kSecAttrKeyType key with a value of any key type defined in `SecItem.h` (see Keychain services), for example, kSecAttrKeyTypeRSA.

- A kSecAttrKeySizeInBits key with a value specifying the requested key size in bits. This can be specified as either a `CFNumberRef` or `CFStringRef` value. For example, RSA keys may have key size values of 512, 768, 1024, or 2048.

In addition, you can specify a number of other optional attributes for the public and private keys. The way you do this depends on whether you are writing code for macOS or iOS:

- In macOS, add the key-value pairs to the `parameters` dictionary directly. The specified attributes are applied to both the public and private keys.

- In iOS, add dictionaries for the keys kSecPublicKeyAttrs and kSecPrivateKeyAttrs to the `parameters` dictionary, and provide the attributes in those dictionaries. The attributes specified in these dictionaries are added to either the public or private key, respectively, allowing you to apply separate attributes to each key.

The possible attributes are as follows; for details on each attribute, see Keychain services:

- kSecAttrLabel—Default `NULL`.

- kSecAttrIsPermanent—If this key is present and has a Boolean value of `true`, the key or key pair is added to the default    keychain.

- kSecAttrApplicationTag—Default `NULL`.

- kSecAttrEffectiveKeySize—Default (`NULL`) sets the effective key size to the same as the total key size (`kSecAttrKeySizeInBits`).

- kSecAttrCanEncrypt—Default `false` for private keys, `true` for public keys.

- kSecAttrCanDecrypt—Default `true` for private keys, `false` for public keys.

- kSecAttrCanDerive—Default `true`.

- kSecAttrCanSign—Default `true` for private keys, `false` for public keys.

- kSecAttrCanVerify—Default `false` for private keys, `true` for public keys.

- kSecAttrCanUnwrap—Default `true` for private keys, `false` for public keys.

