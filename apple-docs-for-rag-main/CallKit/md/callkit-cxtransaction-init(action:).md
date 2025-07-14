

- CallKit
- CXTransaction
-  init(action:) 

Initializer

# init(action:)

Initializes a new transaction with the specified action.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init(action: CXAction)
```

## Parameters 

`action`  

The action to add to the transaction.

## Return Value

A new transaction with the specified action.

## Discussion

This initializer is a convenience for using the designated initializer and calling the addAction(_:) method passing `action`.

## See Also

### Creating New Transactions

init(actions: [CXAction])

Initializes a new transaction with the specified actions.

