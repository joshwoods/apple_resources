

- ProximityReader
- PaymentCardReader
-  fetchPaymentCardReaderStore() 

Instance Method

# fetchPaymentCardReaderStore()

Returns a store containing the read results the framework obtained using a Store and Forward session.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
func fetchPaymentCardReaderStore() throws -> PaymentCardReaderStore
```

## Return Value

PaymentCardReaderStore when successful.

## Discussion

Throws

PaymentCardReaderError if the method fails to retrieve the store.

