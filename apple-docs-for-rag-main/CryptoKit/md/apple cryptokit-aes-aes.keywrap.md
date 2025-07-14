

- Apple CryptoKit
- AES
-  AES.KeyWrap 

Enumeration

# AES.KeyWrap

An implementation of AES Key Wrapping in accordance with the IETF RFC 3394 specification.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum KeyWrap
```

## Topics

### Wrapping an AES key

static func wrap(SymmetricKey, using: SymmetricKey) throws -> Data

Wraps a key using the AES wrap algorithm.

### Unwrapping an AES key

static func unwrap&lt;WrappedKey>(WrappedKey, using: SymmetricKey) throws -> SymmetricKey

Unwraps a key using the AES wrap algorithm.

## Relationships

### Conforms To

- Sendable

