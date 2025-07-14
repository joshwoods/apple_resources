

- ProximityReader
- StoreAndForwardPaymentCardReaderSession
-  status() 

Instance Method

# status()

Allows the merchant to check the status of the Store and Forward session.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
func status() async throws -> StoreAndForwardStatus
```

## Return Value

StoreAndForwardStatus when successful.

## Discussion

Throws

This method throws a `ReadError` if status cannot be retrieved.

