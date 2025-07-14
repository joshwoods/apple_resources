

- Apple CryptoKit
- AES
-  AES.GCM 

Enumeration

# AES.GCM

The Advanced Encryption Standard (AES) Galois Counter Mode (GCM) cipher suite.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum GCM
```

## Topics

### Storing the output

struct SealedBox

A secure container for your data that you can access using a cipher.

### Getting a nonce

struct Nonce

A value used once during a cryptographic operation and then discarded.

### Securing the plaintext message

static func seal&lt;Plaintext>(Plaintext, using: SymmetricKey, nonce: AES.GCM.Nonce?) throws -> AES.GCM.SealedBox

Secures the given plaintext message with encryption and an authentication tag.

static func seal&lt;Plaintext, AuthenticatedData>(Plaintext, using: SymmetricKey, nonce: AES.GCM.Nonce?, authenticating: AuthenticatedData) throws -> AES.GCM.SealedBox

Secures the given plaintext message with encryption and an authentication tag that covers both the encrypted data and additional data.

### Decrypting and verifying the message

static func open(AES.GCM.SealedBox, using: SymmetricKey) throws -> Data

Decrypts the message and verifies its authenticity.

static func open&lt;AuthenticatedData>(AES.GCM.SealedBox, using: SymmetricKey, authenticating: AuthenticatedData) throws -> Data

Decrypts the message and verifies the authenticity of both the encrypted message and additional data.

## Relationships

### Conforms To

- Sendable

