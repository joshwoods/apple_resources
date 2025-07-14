

- Apple CryptoKit
- AES
- AES.GCM
-  seal(\_:using:nonce:) 

Type Method

# seal(\_:using:nonce:)

Secures the given plaintext message with encryption and an authentication tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func seal(
    _ message: Plaintext,
    using key: SymmetricKey,
    nonce: AES.GCM.Nonce? = nil
) throws -> AES.GCM.SealedBox where Plaintext : DataProtocol
```

## Parameters 

`message`  

The plaintext data to seal.

`key`  

A cryptographic key used to seal the message.

`nonce`  

The nonce the sealing process requires. If you don’t provide a nonce, the method generates a random one by invoking `AES.GCM.Nonce()`.

## Return Value

The sealed message.

## See Also

### Securing the plaintext message

static func seal&lt;Plaintext, AuthenticatedData>(Plaintext, using: SymmetricKey, nonce: AES.GCM.Nonce?, authenticating: AuthenticatedData) throws -> AES.GCM.SealedBox

Secures the given plaintext message with encryption and an authentication tag that covers both the encrypted data and additional data.

