

- Apple CryptoKit
- Curve25519
- Curve25519.KeyAgreement
- Curve25519.KeyAgreement.PublicKey
-  init(\_:kem:) 

Initializer

# init(\_:kem:)

Creates a Curve25519 elliptic curve public key for use with Diffie-Hellman key exchange.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    _ serialization: D,
    kem: HPKE.KEM
) throws where D : ContiguousBytes
```

## Discussion

- serialization: The serialized bytes of the public key.

- kem: The key encapsulation mechanism to use with the public key.

Throws

HPKE.Errors.inconsistentCiphersuiteAndKey if the key encapsulation mechanism requested is incompatible with this public key.

