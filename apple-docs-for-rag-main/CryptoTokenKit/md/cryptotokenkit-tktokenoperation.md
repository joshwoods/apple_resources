

- CryptoTokenKit
-  TKTokenOperation 

Enumeration

# TKTokenOperation

Operations that can be performed with a token’s keys and certificates.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum TKTokenOperation
```

## Topics

### Constants

case none

case readData

case signData

case decryptData

case performKeyExchange

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining Support for Operations

func tokenSession(TKTokenSession, supports: TKTokenOperation, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm) -> Bool

Asks the delegate whether the token session supports a given operation using the specified key and algorithm.

typealias ObjectID

A unique and persistent identifier of a particular token object.

class TKTokenKeyAlgorithm

Cryptographic algorithms used by token keys.

