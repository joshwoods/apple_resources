

- ProximityReader
- PaymentCardReadResult
-  paymentCardData 

Instance Property

# paymentCardData

A Base64-encoded string that contains the encrypted payment information to send to your payment provider.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
let paymentCardData: String?
```

## Mentioned in 

Adding support for Tap to Pay on iPhone to your app

## Discussion

This information is present any time the system reads a card, including for purchases, refunds, and card verification.

## See Also

### Getting the result data

let generalCardData: String?

A Base64-encoded string that contains general cardholder and terminal data in tag-length-value (TLV) format.

