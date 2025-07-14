

- CryptoTokenKit
-  TKTokenPasswordAuthOperation 

Class

# TKTokenPasswordAuthOperation

A password-based authentication operation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTokenPasswordAuthOperation
```

## Topics

### Managing the Password

var password: String?

The password to be filled in when the `finishWithError:` is called.

## Relationships

### Inherits From

- TKTokenAuthOperation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Authenticating

func tokenSession(TKTokenSession, beginAuthFor: TKTokenOperation, constraint: Any) throws -> TKTokenAuthOperation

Tells the delegate that authentication has begun for the specified operation and constraint.

typealias TKTokenOperationConstraint

A token’s authentication constraint for a specific operation.

class TKTokenAuthOperation

An authentication operation for a cryptographic token.

class TKTokenSmartCardPINAuthOperation

A Smart Card PIN authentication operation.

