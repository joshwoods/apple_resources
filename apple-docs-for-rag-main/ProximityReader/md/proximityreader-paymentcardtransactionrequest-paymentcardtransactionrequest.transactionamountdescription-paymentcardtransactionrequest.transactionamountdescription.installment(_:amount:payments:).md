

- ProximityReader
- PaymentCardTransactionRequest
- PaymentCardTransactionRequest.TransactionAmountDescription
-  PaymentCardTransactionRequest.TransactionAmountDescription.installment(\_:amount:payments:) 

Case

# PaymentCardTransactionRequest.TransactionAmountDescription.installment(\_:amount:payments:)

The total amount authorized upfront. The customer pays the specified amount on each payment cycle. Only allowed for PaymentCardTransactionRequest.TransactionType.purchase

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
case installment(
    PaymentCardTransactionRequest.PaymentCycle,
    amount: Decimal,
    payments: Int
)
```

## Parameters 

`amount`  

The amount the payment processor deducts from the card for each installment.

`payments`  

The number of payments for the deducted amount. Must be greater than `0`, otherwise the description won’t appear in the UI.

