

- Apple CryptoKit
- HPKE
- HPKE.Sender
-  init(recipientKey:ciphersuite:info:authenticatedBy:presharedKey:presharedKeyIdentifier:) 

Initializer

# init(recipientKey:ciphersuite:info:authenticatedBy:presharedKey:presharedKeyIdentifier:)

Creates a sender in authentication and preshared key mode.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    recipientKey: SK.PublicKey,
    ciphersuite: HPKE.Ciphersuite,
    info: Data,
    authenticatedBy authenticationKey: SK,
    presharedKey psk: SymmetricKey,
    presharedKeyIdentifier pskID: Data
) throws where SK : HPKEDiffieHellmanPrivateKey
```

## Parameters 

`recipientKey`  

The recipient’s public key for encrypting the messages.

`ciphersuite`  

The cipher suite that defines the cryptographic algorithms to use.

`info`  

Data that the key derivation function uses to compute the symmetric key material. The sender and the recipient need to use the same `info` data.

`authenticationKey`  

The sender’s private key for generating the HMAC.

`psk`  

A preshared key (PSK) that the sender and the recipient both hold.

`pskID`  

An identifier for the PSK.

## Discussion

The `Sender` encrypts messages in authentication and preshared key (`auth_psk`) mode using a symmetric encryption key that the sender and recipient both know in advance, in combination with a key it derives using a key derivation function (KDF) and the key schedule data in `info`. Messages also include authentication data so that the recipient can verify the authenticity of the sender’s private key.

Note

The system throws errors from HPKE.Errors when it encounters them.

