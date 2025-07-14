

- Apple CryptoKit
- HPKE
- HPKE.Sender
-  seal(\_:authenticating:) 

Instance Method

# seal(\_:authenticating:)

Encrypts the given cleartext message and attaches additional authenticated data.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
mutating func seal(
    _ msg: M,
    authenticating aad: AD
) throws -> Data where M : DataProtocol, AD : DataProtocol
```

## Parameters 

`msg`  

The cleartext message to encrypt.

`aad`  

Additional data that the `Sender` authenticates and adds to the message in cleartext.

## Return Value

The ciphertext for the recipient to decrypt.

## Discussion

You can call this method multiple times to encrypt a series of messages. When using this method, you need to supply ciphertext messages to the decryption code on the receiving side in the same order as you encrypt them.

Note

The system throws errors from HPKE.Errors when it encounters them.

