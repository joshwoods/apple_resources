

- ProximityReader
- StoreAndForwardPaymentCardReaderSession
-  decline() 

Instance Method

# decline()

Removes the last read from store.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
func decline() async throws
```

## Discussion

This method should be used after a read, when the merchant receives the PaymentCardReadResult and decides to not accept the payment. It must be called within the 60 seconds allowance time window and the payment must not have been included in a batch, otherwise an error will be thrown.

Throws

This method throws a `ReadError` if no previous read was executed, if invoked after the 60 seconds allowance time window or if the payment you are trying to decline belongs to a batch.

