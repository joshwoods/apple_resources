

- Apple CryptoKit
- HPKE
- HPKE.Sender
-  init(recipientKey:ciphersuite:info:presharedKey:presharedKeyIdentifier:) 

Initializer

# init(recipientKey:ciphersuite:info:presharedKey:presharedKeyIdentifier:)

Creates a sender in preshared key (PSK) mode.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    recipientKey: PK,
    ciphersuite: HPKE.Ciphersuite,
    info: Data,
    presharedKey psk: SymmetricKey,
    presharedKeyIdentifier pskID: Data
) throws where PK : HPKEDiffieHellmanPublicKey
```

## Parameters 

`recipientKey`  

The recipient’s public key for encrypting the messages.

`ciphersuite`  

The cipher suite that defines the cryptographic algorithms to use.

`info`  

Data that the key derivation function uses to compute the symmetric key material. The sender and the recipient need to use the same `info` data.

`psk`  

A preshared key (PSK) that the sender and the recipient both hold.

`pskID`  

An identifier for the PSK.

## Discussion

The `Sender` encrypts messages in PSK mode using a symmetric encryption key that the sender and recipient both know in advance, in combination with a key it derives using a key derivation function (KDF) and the key schedule data in `info`. The `Sender` encapsulates the derived key using the recipient’s public key. You access the encapsulated key using encapsulatedKey.

Note

The system throws errors from HPKE.Errors when it encounters them.

