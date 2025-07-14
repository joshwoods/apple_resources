

- ProximityReader
- PaymentCardTransactionRequest
-  transactionDescription 

Instance Property

# transactionDescription

An optional description of the current transaction meant to provide more context, such as a recurring payment being setup or a surcharge applied.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
var transactionDescription: PaymentCardTransactionRequest.TransactionAmountDescription?
```

## Discussion

This attribute is only displayed when the PaymentCardTransactionRequest.TransactionType is compatible with the PaymentCardTransactionRequest.TransactionAmountDescription use case.

## See Also

### Getting the transaction details

let amount: Decimal

The amount of the purchase or refund in the specified currency.

let currencyCode: String

The ISO 4217 code that indicates the currency type.

let type: PaymentCardTransactionRequest.TransactionType

The type of transaction, either a purchase or a refund.

enum TransactionType

The type of transaction to perform.

enum TransactionAmountDescription

Values that provide additional information about the transaction amount.

