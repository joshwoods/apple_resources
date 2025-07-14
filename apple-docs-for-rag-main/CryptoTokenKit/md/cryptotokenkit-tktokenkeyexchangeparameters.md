

- CryptoTokenKit
-  TKTokenKeyExchangeParameters 

Class

# TKTokenKeyExchangeParameters

Parameters used to perform specific key exchange operations.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTokenKeyExchangeParameters
```

## Topics

### Accessing Parameters

var requestedSize: Int

Returns the requested output size, in bytes, of key exchange result.

var sharedInfo: Data?

Returns shared information typically used during the key derivation (KDF) step of a key exchange algorithm.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Performing Cryptographic Operations

func tokenSession(TKTokenSession, sign: Data, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm) throws -> Data

Tells the delegate to sign a data object using the specified key and algorithm.

func tokenSession(TKTokenSession, decrypt: Data, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm) throws -> Data

Tells the delegate to decrypt a data object using the specified key and algorithm.

func tokenSession(TKTokenSession, performKeyExchange: Data, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm, parameters: TKTokenKeyExchangeParameters) throws -> Data

Tells the delegate to perform a key exchange using the specified key and algorithm.

