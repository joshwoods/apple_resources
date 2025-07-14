

- StoreKit Test
- SKTestSession
-  approveAskToBuyTransaction(identifier:) 

Instance Method

# approveAskToBuyTransaction(identifier:)

Resolves an Ask to Buy test scenario by approving the transaction.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func approveAskToBuyTransaction(identifier: Int) throws
```

## Parameters 

`identifier`  

The transaction identifier of the Ask to Buy transaction.

## See Also

### Testing Ask To Buy transactions

var askToBuyEnabled: Bool

A Boolean value that determines whether the testing environment simulates an Ask to Buy scenario.

func declineAskToBuyTransaction(identifier: Int) throws

Resolves an Ask to Buy test scenario by declining the transaction.

