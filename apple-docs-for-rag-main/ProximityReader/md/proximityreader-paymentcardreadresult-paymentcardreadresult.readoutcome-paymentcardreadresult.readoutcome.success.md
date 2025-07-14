

- ProximityReader
- PaymentCardReadResult
- PaymentCardReadResult.ReadOutcome
-  PaymentCardReadResult.ReadOutcome.success 

Case

# PaymentCardReadResult.ReadOutcome.success

The read was successful.

iOS 16.4+iPadOS 16.4+Mac Catalyst 17.0+

``` source
case success
```

## See Also

### Getting the read outcome

case failure

The read failed somehow, the card data may not contain all requested tags.

case cardDeclined

The card declined this transaction.

