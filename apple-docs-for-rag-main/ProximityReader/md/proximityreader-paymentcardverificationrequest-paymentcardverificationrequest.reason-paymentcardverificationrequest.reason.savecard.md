

- ProximityReader
- PaymentCardVerificationRequest
- PaymentCardVerificationRequest.Reason
-  PaymentCardVerificationRequest.Reason.saveCard 

Case

# PaymentCardVerificationRequest.Reason.saveCard

Save the card information for later.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
case saveCard
```

## Discussion

If your application saves card data, it’s your responsibility to ensure that the customer is aware of how and why before you read their card.

## See Also

### Getting the verification reason

case lookUp

Verify the payment card to look up a past transaction.

case openTab

Check if the card is valid.

case other

Verify the card information.

