

- CryptoTokenKit
- TKTokenSessionDelegate
-  tokenSession(\_:sign:keyObjectID:algorithm:) 

Instance Method

# tokenSession(\_:sign:keyObjectID:algorithm:)

Tells the delegate to sign a data object using the specified key and algorithm.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional func tokenSession(
    _ session: TKTokenSession,
    sign dataToSign: Data,
    keyObjectID: TKToken.ObjectID,
    algorithm: TKTokenKeyAlgorithm
) throws -> Data
```

## Parameters 

`session`  

The token session.

`dataToSign`  

The data to sign.

`keyObjectID`  

The identifier of the private key object.

`algorithm`  

The algorithm to be used for signing.

## Return Value

The signed data, or `nil` if an error occurred.

## See Also

### Performing Cryptographic Operations

func tokenSession(TKTokenSession, decrypt: Data, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm) throws -> Data

Tells the delegate to decrypt a data object using the specified key and algorithm.

func tokenSession(TKTokenSession, performKeyExchange: Data, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm, parameters: TKTokenKeyExchangeParameters) throws -> Data

Tells the delegate to perform a key exchange using the specified key and algorithm.

class TKTokenKeyExchangeParameters

Parameters used to perform specific key exchange operations.

