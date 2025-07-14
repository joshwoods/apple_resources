

- ProximityReader
- StoreAndForwardBatch
- StoreAndForwardBatch.StoredPaymentCardReadResult
-  paymentCardData 

Instance Property

# paymentCardData

A Base64-encoded string that contains the encrypted payment information to send to your payment provider.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
let paymentCardData: String
```

## Discussion

This information is present any time the system reads a card, including for purchases, refunds, and card verification.

