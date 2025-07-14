

- ProximityReader
- PaymentCardReaderStore
-  resolveBatch(batchDeletionToken:) 

Instance Method

# resolveBatch(batchDeletionToken:)

Deletes the current batch and all its Store and Forward payments, allowing you to request a new batch.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
func resolveBatch(batchDeletionToken: StoreAndForwardBatchDeletionToken) async throws -> Int
```

## Parameters 

`batchDeletionToken`  

The token you receive from the payment service provider.

## Return Value

The remaining number of payments to process.

## Discussion

Throws

This method throws a PaymentCardReaderStore.StoreError if the customer isn’t online at the moment you call it, if there’s no Store and Forward batch to resolve, or if the deletion token is invalid.

