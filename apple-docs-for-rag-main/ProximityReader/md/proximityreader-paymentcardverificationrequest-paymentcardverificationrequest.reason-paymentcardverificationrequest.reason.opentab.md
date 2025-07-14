

- ProximityReader
- PaymentCardVerificationRequest
- PaymentCardVerificationRequest.Reason
-  PaymentCardVerificationRequest.Reason.openTab 

Case

# PaymentCardVerificationRequest.Reason.openTab

Check if the card is valid.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
case openTab
```

## Discussion

Choose this reason when you aren’t ready to complete the purchase yet, but want to verify that the person’s credit card information is valid.

## See Also

### Getting the verification reason

case lookUp

Verify the payment card to look up a past transaction.

case saveCard

Save the card information for later.

case other

Verify the card information.

