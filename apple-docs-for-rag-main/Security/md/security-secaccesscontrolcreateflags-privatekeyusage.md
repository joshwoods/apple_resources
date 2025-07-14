

- Security
- SecAccessControlCreateFlags
-  privateKeyUsage 

Type Property

# privateKeyUsage

Enable a private key to be used in signing a block of data or verifying a signed block.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var privateKeyUsage: SecAccessControlCreateFlags { get }
```

## Mentioned in 

Protecting keys with the Secure Enclave

## Discussion

This option can be combined with any other access control flags.

You typically use this constraint when you create a key pair and store the private key inside a device’s Secure Enclave (by specifying the kSecAttrTokenID attribute with a value of kSecAttrTokenIDSecureEnclave). This makes the private key available for use in signing and verification tasks that happen inside the Secure Enclave with calls to the SecKeyRawSign(_:_:_:_:_:_:) and SecKeyRawVerify(_:_:_:_:_:_:) functions. An attempt to use this constraint while generating a key pair outside the Secure Enclave fails. Similarly, an attempt to sign a block with a private key generated without this constraint inside the Secure Enclave fails.

