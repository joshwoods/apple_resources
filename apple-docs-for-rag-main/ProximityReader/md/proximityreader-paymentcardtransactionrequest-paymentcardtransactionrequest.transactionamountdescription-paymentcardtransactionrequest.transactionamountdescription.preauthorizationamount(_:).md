

- ProximityReader
- PaymentCardTransactionRequest
- PaymentCardTransactionRequest.TransactionAmountDescription
-  PaymentCardTransactionRequest.TransactionAmountDescription.preauthorizationAmount(\_:) 

Case

# PaymentCardTransactionRequest.TransactionAmountDescription.preauthorizationAmount(\_:)

Places a temporary hold on the customer’s account for the specified amount. Only allowed for PaymentCardTransactionRequest.TransactionType.purchase

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
case preauthorizationAmount(Decimal)
```

