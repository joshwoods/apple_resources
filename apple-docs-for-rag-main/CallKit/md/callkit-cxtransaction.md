

- CallKit
-  CXTransaction 

Class

# CXTransaction

An object that contains zero or more action objects for a call controller to perform.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXTransaction
```

## Topics

### Creating New Transactions

convenience init(action: CXAction)

Initializes a new transaction with the specified action.

init(actions: [CXAction])

Initializes a new transaction with the specified actions.

### Accessing Transaction Attributes

var uuid: UUID

The unique identifier of the transaction.

var isComplete: Bool

A Boolean value that indicates whether the transaction has been completed.

var actions: [CXAction]

The actions added to a transaction.

### Adding Actions

func addAction(CXAction)

Adds the specified action to the transaction.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Outgoing calls

Sending End-to-End Encrypted VoIP Calls

Initiate VoIP calls when your server can’t determine whether an outgoing notification is a request for a VoIP call due to metadata encryption.

class CXCallController

A programmatic interface for interacting with and observing calls.

class CXStartCallAction

An encapsulation of the act of initiating an outgoing call.

