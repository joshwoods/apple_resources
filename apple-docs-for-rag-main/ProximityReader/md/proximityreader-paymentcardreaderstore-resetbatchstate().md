

- ProximityReader
- PaymentCardReaderStore
-  resetBatchState() 

Instance Method

# resetBatchState()

Resets the current batch state in the store, allowing you to request a new batch.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
func resetBatchState() async throws
```

## Discussion

Use this method if the transmission of the batch to the partner service provider fails and the batch processing status is unknown. The framework doesn’t delete the reads; instead, it dissociates them from the batch.

Throws

This method throws a PaymentCardReaderStore.StoreError if there’s no batch for the framework to reset.

