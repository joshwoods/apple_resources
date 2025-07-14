

- CryptoTokenKit
-  TKTokenSmartCardPINAuthOperation 

Class

# TKTokenSmartCardPINAuthOperation

A Smart Card PIN authentication operation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTokenSmartCardPINAuthOperation
```

## Topics

### Configuring the Operation

var pinFormat: TKSmartCardPINFormat

The PIN format.

var apduTemplate: Data?

The template into which the PIN is filled in. `nil` by default.

var pinByteOffset: Int

The offset, in bytes, within the APDU template to mark the location for filling in the PIN.

var smartCard: TKSmartCard?

A Smart Card to which the formatted APDU is sent in order to authenticate.

### Accessing the PIN

var pin: String?

The PIN value resulting from performing the operation.

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

class TKTokenPasswordAuthOperation

A password-based authentication operation.

