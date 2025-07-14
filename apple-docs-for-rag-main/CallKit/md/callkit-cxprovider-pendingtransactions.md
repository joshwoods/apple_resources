

- CallKit
- CXProvider
-  pendingTransactions 

Instance Property

# pendingTransactions

Incomplete transactions.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
var pendingTransactions: [CXTransaction] { get }
```

## See Also

### Accessing Pending Transaction and Call Actions

func pendingCallActions(of: AnyClass, withCall: UUID) -> [CXCallAction]

Returns all call actions in any pending transactions of the specified class for the specified call identifier that are incomplete.

