

- CryptoTokenKit
-  TKTokenAuthOperation 

Class

# TKTokenAuthOperation

An authentication operation for a cryptographic token.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTokenAuthOperation
```

## Overview

The CryptoTokenKit framework provides the following concrete subclasses: TKTokenPasswordAuthOperation, for password-based authentication, and TKTokenSmartCardPINAuthOperation for Smart Card PIN-based authentication.

## Topics

### Finishing the Operation

func finish() throws

Finishes the authentication operation.

## Relationships

### Inherits From

- NSObject

### Inherited By

- TKTokenPasswordAuthOperation
- TKTokenSmartCardPINAuthOperation

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

class TKTokenPasswordAuthOperation

A password-based authentication operation.

class TKTokenSmartCardPINAuthOperation

A Smart Card PIN authentication operation.

