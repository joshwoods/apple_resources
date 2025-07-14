

- Security
-  kSecAttrTokenID 

Global Variable

# kSecAttrTokenID

A key whose value indicates that a cryptographic key is in an external store.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrTokenID: CFString
```

## Mentioned in 

Protecting keys with the Secure Enclave

## Discussion

The corresponding value is of type CFString, and may only be one of the constants specified in Token ID Values. Presence of this key indicates that the item is backed by an external store, as uniquely identified by the value. An item without this attribute is stored as normal in the keychain database.

Important

You can’t change this attribute after creating the keychain item. It isn’t possible to migrate existing items between stores. Setting `kSecAttrTokenID` when creating a keychain item in macOS makes it behave like an iOS keychain item, as if kSecAttrSynchronizable were also set.

Use this attribute only in the top-level parameter dictionary during key creation and not in one of the private or public key sub-dictionaries given by kSecPrivateKeyAttrs or kSecPublicKeyAttrs, respectively. For an example, see Protecting keys with the Secure Enclave.

