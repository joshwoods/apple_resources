

- ProximityReader
- PaymentCardReadResult
- PaymentCardReadResult.ReadOutcome
-  PaymentCardReadResult.ReadOutcome.failure 

Case

# PaymentCardReadResult.ReadOutcome.failure

The read failed somehow, the card data may not contain all requested tags.

iOS 16.4+iPadOS 16.4+Mac Catalyst 17.0+

``` source
case failure
```

## See Also

### Getting the read outcome

case success

The read was successful.

case cardDeclined

The card declined this transaction.

