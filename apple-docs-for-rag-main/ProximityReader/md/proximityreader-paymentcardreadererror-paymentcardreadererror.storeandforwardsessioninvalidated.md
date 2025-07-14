

- ProximityReader
- PaymentCardReaderError
-  PaymentCardReaderError.storeAndForwardSessionInvalidated 

Case

# PaymentCardReaderError.storeAndForwardSessionInvalidated

An error that indicates the framework invalidated the current Store and Forward session, and it can’t execute additional reads.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
case storeAndForwardSessionInvalidated
```

## Discussion

You must prepare an online session and prepare a new Store and Forward session.

