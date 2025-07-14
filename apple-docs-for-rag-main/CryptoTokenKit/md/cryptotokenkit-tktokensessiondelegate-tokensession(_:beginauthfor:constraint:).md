

- CryptoTokenKit
- TKTokenSessionDelegate
-  tokenSession(\_:beginAuthFor:constraint:) 

Instance Method

# tokenSession(\_:beginAuthFor:constraint:)

Tells the delegate that authentication has begun for the specified operation and constraint.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional func tokenSession(
    _ session: TKTokenSession,
    beginAuthFor operation: TKTokenOperation,
    constraint: Any
) throws -> TKTokenAuthOperation
```

## Parameters 

`session`  

The token session.

`operation`  

The kind of operation.

`constraint`  

The constraint to be satisfied.

## Return Value

The resulting context of the operation, or `nil` if an error occurred.

## Discussion

If you return an instance of a subclass of TKTokenAuthOperation that is provided by the CryptoTokenKit framework, the system will first fill in the context-specific properties, such as the password, before calling the `finishWithError:` method on the context.

## See Also

### Authenticating

typealias TKTokenOperationConstraint

A token’s authentication constraint for a specific operation.

class TKTokenAuthOperation

An authentication operation for a cryptographic token.

class TKTokenPasswordAuthOperation

A password-based authentication operation.

class TKTokenSmartCardPINAuthOperation

A Smart Card PIN authentication operation.

