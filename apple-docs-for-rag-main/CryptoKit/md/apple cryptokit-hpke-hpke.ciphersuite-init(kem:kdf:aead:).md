

- Apple CryptoKit
- HPKE
- HPKE.Ciphersuite
-  init(kem:kdf:aead:) 

Initializer

# init(kem:kdf:aead:)

Creates an HPKE cipher suite.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    kem: HPKE.KEM,
    kdf: HPKE.KDF,
    aead: HPKE.AEAD
)
```

## Parameters 

`kem`  

The key encapsulation mechanism for encapsulating the symmetric key.

`kdf`  

The key derivation function for deriving the symmetric key.

`aead`  

The authenticated encryption with additional data (AEAD) algorithm for encrypting and decrypting messages.

