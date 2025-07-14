

- CryptoTokenKit
- TKTokenSessionDelegate
-  tokenSession(\_:decrypt:keyObjectID:algorithm:) 

Instance Method

# tokenSession(\_:decrypt:keyObjectID:algorithm:)

Tells the delegate to decrypt a data object using the specified key and algorithm.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional func tokenSession(
    _ session: TKTokenSession,
    decrypt ciphertext: Data,
    keyObjectID: TKToken.ObjectID,
    algorithm: TKTokenKeyAlgorithm
) throws -> Data
```

## Parameters 

`session`  

The token session.

`ciphertext`  

The data to decrypt.

`keyObjectID`  

The identifier of the public key object.

`algorithm`  

The algorithm to be used for decryption.

## Return Value

The decrypted data, or `nil` if an error occurred.

## See Also

### Performing Cryptographic Operations

func tokenSession(TKTokenSession, sign: Data, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm) throws -> Data

Tells the delegate to sign a data object using the specified key and algorithm.

func tokenSession(TKTokenSession, performKeyExchange: Data, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm, parameters: TKTokenKeyExchangeParameters) throws -> Data

Tells the delegate to perform a key exchange using the specified key and algorithm.

class TKTokenKeyExchangeParameters

Parameters used to perform specific key exchange operations.

