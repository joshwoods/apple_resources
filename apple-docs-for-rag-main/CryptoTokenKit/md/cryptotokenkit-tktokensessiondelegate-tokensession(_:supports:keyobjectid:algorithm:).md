

- CryptoTokenKit
- TKTokenSessionDelegate
-  tokenSession(\_:supports:keyObjectID:algorithm:) 

Instance Method

# tokenSession(\_:supports:keyObjectID:algorithm:)

Asks the delegate whether the token session supports a given operation using the specified key and algorithm.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional func tokenSession(
    _ session: TKTokenSession,
    supports operation: TKTokenOperation,
    keyObjectID: TKToken.ObjectID,
    algorithm: TKTokenKeyAlgorithm
) -> Bool
```

## Parameters 

`session`  

The token session.

`operation`  

The operation to perform. For possible values, see `TKTokenOperation`.

`keyObjectID`  

The identifier of the private key object.

`algorithm`  

The algorithm to be used by the operation.

## Return Value

true if the operation is supported; otherwise, false.

## See Also

### Determining Support for Operations

enum TKTokenOperation

Operations that can be performed with a token’s keys and certificates.

typealias ObjectID

A unique and persistent identifier of a particular token object.

class TKTokenKeyAlgorithm

Cryptographic algorithms used by token keys.

