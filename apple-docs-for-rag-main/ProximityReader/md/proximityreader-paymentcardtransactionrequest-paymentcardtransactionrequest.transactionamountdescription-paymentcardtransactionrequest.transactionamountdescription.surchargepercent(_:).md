

- ProximityReader
- PaymentCardTransactionRequest
- PaymentCardTransactionRequest.TransactionAmountDescription
-  PaymentCardTransactionRequest.TransactionAmountDescription.surchargePercent(\_:) 

Case

# PaymentCardTransactionRequest.TransactionAmountDescription.surchargePercent(\_:)

The maximum surcharge percentage the payment processor may apply to the transaction. Only allowed for PaymentCardTransactionRequest.TransactionType.purchase

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
case surchargePercent(Double)
```

## Discussion

The payment processor determines the final surcharge amount when they process the transaction. The percentage value is between 1 and 100 and up to two decimal places.

