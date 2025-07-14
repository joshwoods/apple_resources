

- ProximityReader
- PaymentCardReaderStore
-  fetchStoredPaymentCardReadResultBatch(size:) 

Instance Method

# fetchStoredPaymentCardReadResultBatch(size:)

Returns a batch of reads the framework previously stored, in chronological order, of the size you request.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
func fetchStoredPaymentCardReadResultBatch(size: Int = 0) async throws -> StoreAndForwardBatch
```

## Parameters 

`size`  

The desired batch size, if no size is provided, the framework uses a batch size of `0` that returns all the payments stored in the batch.

## Return Value

StoreAndForwardBatch when successful.

## Discussion

There is only one active batch per application at a given time and to fetch a new batch the caller needs to reset or resolve the current batch.

Throws

This method throws a PaymentCardReaderStore.StoreError if the size is smaller than `0` or greater than the number of payments stored, or if there’s no payment stored. The framework also throws a `StoreError` if a previous batch is pending resolution at the time when you call this method.

