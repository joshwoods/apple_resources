

- CallKit
- CXTransaction
-  isComplete 

Instance Property

# isComplete

A Boolean value that indicates whether the transaction has been completed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
var isComplete: Bool { get }
```

## Discussion

A transaction is complete only when all of its actions are complete.

## See Also

### Accessing Transaction Attributes

var uuid: UUID

The unique identifier of the transaction.

var actions: [CXAction]

The actions added to a transaction.

