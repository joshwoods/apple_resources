

- ProximityReader
- PaymentCardReaderError
-  PaymentCardReaderError.storeAndForwardTokenIssuerChanged 

Case

# PaymentCardReaderError.storeAndForwardTokenIssuerChanged

An error that indicates the current Store and Forward mode has payments from a different token issuer.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
case storeAndForwardTokenIssuerChanged
```

## Discussion

You must process the previous token issuer payments and create a new Store and Forward session.

