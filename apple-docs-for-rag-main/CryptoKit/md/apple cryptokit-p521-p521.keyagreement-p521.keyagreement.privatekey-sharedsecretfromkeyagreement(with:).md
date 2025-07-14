

- Apple CryptoKit
- P521
- P521.KeyAgreement
- P521.KeyAgreement.PrivateKey
-  sharedSecretFromKeyAgreement(with:) 

Instance Method

# sharedSecretFromKeyAgreement(with:)

Computes a shared secret with the provided public key from another party.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func sharedSecretFromKeyAgreement(with publicKeyShare: P521.KeyAgreement.PublicKey) throws -> SharedSecret
```

## Parameters 

`publicKeyShare`  

The public key from another party to be combined with the private key from this user to create the shared secret.

## Return Value

The computed shared secret.

## See Also

### Creating a shared secret

struct SharedSecret

A key agreement result from which you can derive a symmetric cryptographic key.

