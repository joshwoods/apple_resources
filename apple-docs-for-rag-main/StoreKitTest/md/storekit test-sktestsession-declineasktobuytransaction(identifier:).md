

- StoreKit Test
- SKTestSession
-  declineAskToBuyTransaction(identifier:) 

Instance Method

# declineAskToBuyTransaction(identifier:)

Resolves an Ask to Buy test scenario by declining the transaction.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func declineAskToBuyTransaction(identifier: Int) throws
```

## Parameters 

`identifier`  

The transaction identifier of an Ask to Buy transaction.

## See Also

### Testing Ask To Buy transactions

var askToBuyEnabled: Bool

A Boolean value that determines whether the testing environment simulates an Ask to Buy scenario.

func approveAskToBuyTransaction(identifier: Int) throws

Resolves an Ask to Buy test scenario by approving the transaction.

