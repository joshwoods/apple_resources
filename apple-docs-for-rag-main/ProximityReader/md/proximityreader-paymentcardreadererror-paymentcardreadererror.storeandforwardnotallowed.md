

- ProximityReader
- PaymentCardReaderError
-  PaymentCardReaderError.storeAndForwardNotAllowed 

Case

# PaymentCardReaderError.storeAndForwardNotAllowed

An error that indicates the framework can’t create a Store and Forward session because:

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
case storeAndForwardNotAllowed
```

## Discussion

- There’s no previous online session.

- The person restarted their phone after the online session creation, and they now require a new online session.

- More than 24 hours have passed since the last online session.

