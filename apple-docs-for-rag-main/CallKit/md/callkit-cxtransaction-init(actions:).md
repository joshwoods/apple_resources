

- CallKit
- CXTransaction
-  init(actions:) 

Initializer

# init(actions:)

Initializes a new transaction with the specified actions.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
init(actions: [CXAction])
```

## Parameters 

`actions`  

The actions to added to the transaction.

## Return Value

A new transaction with the specified actions.

## Discussion

This initializer is a convenience for using the designated initializer and calling the addAction(_:) method passing each object in `actions`.

## See Also

### Creating New Transactions

convenience init(action: CXAction)

Initializes a new transaction with the specified action.

