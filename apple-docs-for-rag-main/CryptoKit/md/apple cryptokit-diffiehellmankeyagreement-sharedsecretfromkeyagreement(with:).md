

- Apple CryptoKit
- DiffieHellmanKeyAgreement
-  sharedSecretFromKeyAgreement(with:) 

Instance Method

# sharedSecretFromKeyAgreement(with:)

Performs a Diffie-Hellman Key Agreement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func sharedSecretFromKeyAgreement(with publicKeyShare: Self.PublicKey) throws -> SharedSecret
```

**Required**

## Parameters 

`publicKeyShare`  

The public key share.

## Return Value

The resulting key agreement result.

