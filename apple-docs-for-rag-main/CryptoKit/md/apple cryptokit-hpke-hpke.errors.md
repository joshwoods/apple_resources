

- Apple CryptoKit
- HPKE
-  HPKE.Errors 

Enumeration

# HPKE.Errors

Hybrid public key encryption (HPKE) errors that CryptoKit uses.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum Errors
```

## Topics

### Enumeration Cases

case ciphertextTooShort

The ciphertext is too short.

case expectedPSK

The PSK is nil and the object is in PSK mode, or in authentication and PSK mode.

case exportOnlyMode

The object is in export-only mode and received a request to encrypt or decrypt data.

case inconsistentCiphersuiteAndKey

The supplied encryption key is incompatible with the requested cipher suite.

case inconsistentPSKInputs

The PSK is nil and the PSK ID isn’t nil, or the PSK ID is nil and the PSK isn’t nil.

case inconsistentParameters

The parameters for initializing an HPKE sender or receiver are inconsistent.

case outOfRangeSequenceNumber

The sequence number for encrypting or decrypting the message is out of range.

case unexpectedPSK

The PSK isn’t nil and the object is in base mode, or in authentication mode.

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

