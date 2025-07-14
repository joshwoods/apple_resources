

- CryptoTokenKit
-  TKTokenOperationConstraint 

Type Alias

# TKTokenOperationConstraint

A token’s authentication constraint for a specific operation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
typealias TKTokenOperationConstraint = AnyObject
```

## Discussion

This object persistently identifies a constraint for performing specific operation on specific object.

- true, indicating that the operation is always allowed, without any authentication necessary.

- false, indicating that the operation is never allowed; this value isn’t typically used.

- Any other property list compatible value defined by the implementation of the token extension. Any such constraint is required to stay constant for the entire lifetime of the token. For example, a Smart Card token extension may decide to use the string constant `"PIN"` to indicate that the operation is authenticated with valid PIN entry to the card.

## See Also

### Authenticating

func tokenSession(TKTokenSession, beginAuthFor: TKTokenOperation, constraint: Any) throws -> TKTokenAuthOperation

Tells the delegate that authentication has begun for the specified operation and constraint.

class TKTokenAuthOperation

An authentication operation for a cryptographic token.

class TKTokenPasswordAuthOperation

A password-based authentication operation.

class TKTokenSmartCardPINAuthOperation

A Smart Card PIN authentication operation.

