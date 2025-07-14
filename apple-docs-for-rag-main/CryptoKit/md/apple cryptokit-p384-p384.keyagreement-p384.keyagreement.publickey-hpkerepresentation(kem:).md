

- Apple CryptoKit
- P384
- P384.KeyAgreement
- P384.KeyAgreement.PublicKey
-  hpkeRepresentation(kem:) 

Instance Method

# hpkeRepresentation(kem:)

Creates a serialized representation of the public key.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func hpkeRepresentation(kem: HPKE.KEM) throws -> Data
```

## Return Value

The serialized representation of the public key.

## Discussion

- kem: The Key Encapsulation Mechanism to use with the public key.

Throws

HPKE.Errors.inconsistentCiphersuiteAndKey if the key encapsulation mechanism requested is incompatible with this public key.

