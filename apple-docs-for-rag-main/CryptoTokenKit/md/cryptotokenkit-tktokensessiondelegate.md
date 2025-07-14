

- CryptoTokenKit
-  TKTokenSessionDelegate 

Protocol

# TKTokenSessionDelegate

The interface that a session instance delegate implements to respond to token session authentication events.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
protocol TKTokenSessionDelegate : NSObjectProtocol
```

## Topics

### Determining Support for Operations

func tokenSession(TKTokenSession, supports: TKTokenOperation, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm) -> Bool

Asks the delegate whether the token session supports a given operation using the specified key and algorithm.

enum TKTokenOperation

Operations that can be performed with a token’s keys and certificates.

typealias ObjectID

A unique and persistent identifier of a particular token object.

class TKTokenKeyAlgorithm

Cryptographic algorithms used by token keys.

### Authenticating

func tokenSession(TKTokenSession, beginAuthFor: TKTokenOperation, constraint: Any) throws -> TKTokenAuthOperation

Tells the delegate that authentication has begun for the specified operation and constraint.

typealias TKTokenOperationConstraint

A token’s authentication constraint for a specific operation.

class TKTokenAuthOperation

An authentication operation for a cryptographic token.

class TKTokenPasswordAuthOperation

A password-based authentication operation.

class TKTokenSmartCardPINAuthOperation

A Smart Card PIN authentication operation.

### Performing Cryptographic Operations

func tokenSession(TKTokenSession, sign: Data, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm) throws -> Data

Tells the delegate to sign a data object using the specified key and algorithm.

func tokenSession(TKTokenSession, decrypt: Data, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm) throws -> Data

Tells the delegate to decrypt a data object using the specified key and algorithm.

func tokenSession(TKTokenSession, performKeyExchange: Data, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm, parameters: TKTokenKeyExchangeParameters) throws -> Data

Tells the delegate to perform a key exchange using the specified key and algorithm.

class TKTokenKeyExchangeParameters

Parameters used to perform specific key exchange operations.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to Authentication Events

var delegate: (any TKTokenSessionDelegate)?

The token session delegate.

