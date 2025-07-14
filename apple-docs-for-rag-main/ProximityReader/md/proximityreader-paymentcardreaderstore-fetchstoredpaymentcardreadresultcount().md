

- ProximityReader
- PaymentCardReaderStore
-  fetchStoredPaymentCardReadResultCount() 

Instance Method

# fetchStoredPaymentCardReadResultCount()

Returns the number of reads the framework performed using a Store and Forward session.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
func fetchStoredPaymentCardReadResultCount() async throws -> Int
```

## Discussion

Throws

This method throws a PaymentCardReaderStore.StoreError if the count cannot be fetched.

