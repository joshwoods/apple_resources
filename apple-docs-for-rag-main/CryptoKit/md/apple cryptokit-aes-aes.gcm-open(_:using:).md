

- Apple CryptoKit
- AES
- AES.GCM
-  open(\_:using:) 

Type Method

# open(\_:using:)

Decrypts the message and verifies its authenticity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func open(
    _ sealedBox: AES.GCM.SealedBox,
    using key: SymmetricKey
) throws -> Data
```

## Parameters 

`sealedBox`  

The sealed box to open.

`key`  

The cryptographic key that was used to seal the message.

## Return Value

The original plaintext message that was sealed in the box, as long as the correct key is used and authentication succeeds. The call throws an error if decryption or authentication fail.

## See Also

### Decrypting and verifying the message

static func open&lt;AuthenticatedData>(AES.GCM.SealedBox, using: SymmetricKey, authenticating: AuthenticatedData) throws -> Data

Decrypts the message and verifies the authenticity of both the encrypted message and additional data.

