

- Apple CryptoKit
- HPKE
- HPKE.Recipient
-  init(privateKey:ciphersuite:info:encapsulatedKey:authenticatedBy:) 

Initializer

# init(privateKey:ciphersuite:info:encapsulatedKey:authenticatedBy:)

Creates a recipient in authentication mode.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    privateKey: SK,
    ciphersuite: HPKE.Ciphersuite,
    info: Data,
    encapsulatedKey: Data,
    authenticatedBy authenticationKey: SK.PublicKey
) throws where SK : HPKEDiffieHellmanPrivateKey
```

## Parameters 

`privateKey`  

The recipient’s private key for decrypting the incoming messages.

`ciphersuite`  

The cipher suite that defines the cryptographic algorithms to use.

`info`  

Data that the key derivation function uses to compute the symmetric key material. The sender and the recipient need to use the same `info` data.

`encapsulatedKey`  

The encapsulated symmetric key that the sender provides.

`authenticationKey`  

The sender’s public key for authenticating the messages.

## Discussion

The `Receiver` decrypts messages in authentication mode using the encapsulated key with the key schedule information (`info` data). Messages also include authentication data so that the recipient can verify the authenticity of the sender’s private key.

Note

The system throws errors from HPKE.Errors when it encounters them.

