

- CryptoTokenKit
- TKTokenSessionDelegate
-  tokenSession(\_:performKeyExchange:keyObjectID:algorithm:parameters:) 

Instance Method

# tokenSession(\_:performKeyExchange:keyObjectID:algorithm:parameters:)

Tells the delegate to perform a key exchange using the specified key and algorithm.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional func tokenSession(
    _ session: TKTokenSession,
    performKeyExchange otherPartyPublicKeyData: Data,
    keyObjectID objectID: TKToken.ObjectID,
    algorithm: TKTokenKeyAlgorithm,
    parameters: TKTokenKeyExchangeParameters
) throws -> Data
```

## Parameters 

`session`  

The token session.

`otherPartyPublicKeyData`  

The public key of the other party.

`objectID`  

The identifier of the private key object.

`algorithm`  

The algorithm to be used for key exchange.

`parameters`  

Additional parameters used by `algorithm` to perform the key exchange.

## Return Value

The result of the key exchange, or `nil` if an error occurred.

## See Also

### Performing Cryptographic Operations

func tokenSession(TKTokenSession, sign: Data, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm) throws -> Data

Tells the delegate to sign a data object using the specified key and algorithm.

func tokenSession(TKTokenSession, decrypt: Data, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm) throws -> Data

Tells the delegate to decrypt a data object using the specified key and algorithm.

class TKTokenKeyExchangeParameters

Parameters used to perform specific key exchange operations.

