

- ProximityReader
- PaymentCardReadResult
- PaymentCardReadResult.ReadOutcome
-  PaymentCardReadResult.ReadOutcome.cardDeclined 

Case

# PaymentCardReadResult.ReadOutcome.cardDeclined

The card declined this transaction.

iOS 16.4+iPadOS 16.4+Mac Catalyst 17.0+

``` source
case cardDeclined
```

## See Also

### Getting the read outcome

case success

The read was successful.

case failure

The read failed somehow, the card data may not contain all requested tags.

