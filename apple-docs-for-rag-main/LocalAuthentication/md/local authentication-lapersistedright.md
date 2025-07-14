

- Local Authentication
-  LAPersistedRight 

Class

# LAPersistedRight

A right that gates access to a key and a secret.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class LAPersistedRight
```

## Overview

An LAPersistedRight is a right that’s backed by a unique key in the Secure Enclave with an access control list that matches the authorization requirements of the right. You can access the key that backs a right to perform cryptographic operations like encryption, decryption, signing, and verification.

You can use the key that backs an LAPersistedRight to perform both public key and private key operations, but private key operations — like decryption, signing, and key exchange — are only available after you authorize the right. Public key operations like encryption and verification are always available.

The following generates a right with the default authorization requirements, stores it in the shared LARightStore, and exports the public key so that you can use it to verify signatures that the corresponding private key produces:

```
func generateClientKeys() async throws -> Data {
    let right = LARight()
    let persistedRight = try await LARightStore.shared.saveRight(right, identifier: "server-access")
    return try await persistedRight.key.publicKey.bytes
}
```

The following uses the private key associated with the right from the previous example to sign a challenge issued by a server:

```
func signServerChallenge(nonce: Data) async throws -> Data {
    let persistedRight = try await LARightStore.shared.right(forIdentifier: "server-access")
    try await persistedRight.authorize(localizedReason: "Access the sandcastle competition server")

    guard persistedRight.key.canSign(using: .ecdsaSignatureMessageX962SHA256) else {
        throw NSError(domain: "ExampleErrorDomain", code: -1, userInfo: [:])
    }

    return try await persistedRight.key.sign(nonce, algorithm: .ecdsaSignatureMessageX962SHA256)
}
```

The signature operation occurs after verifying that the user has the proper authorization and confirming that the private key supports the given signing algorithm.

## Topics

### Accessing persistent data

var key: LAPrivateKey

The private key that’s persisted by the right.

var secret: LASecret

The data kept secret by the right.

## Relationships

### Inherits From

- LARight

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Persistence

class LARightStore

A container for data protected by a right.

class LASecret

Data that’s protected by a persisted right.

