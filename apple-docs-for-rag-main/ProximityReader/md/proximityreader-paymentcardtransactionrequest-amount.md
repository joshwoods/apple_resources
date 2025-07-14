

- ProximityReader
- PaymentCardTransactionRequest
-  amount 

Instance Property

# amount

The amount of the purchase or refund in the specified currency.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
let amount: Decimal
```

## Discussion

The value in this property must be greater than 0.

## See Also

### Getting the transaction details

let currencyCode: String

The ISO 4217 code that indicates the currency type.

let type: PaymentCardTransactionRequest.TransactionType

The type of transaction, either a purchase or a refund.

enum TransactionType

The type of transaction to perform.

var transactionDescription: PaymentCardTransactionRequest.TransactionAmountDescription?

An optional description of the current transaction meant to provide more context, such as a recurring payment being setup or a surcharge applied.

enum TransactionAmountDescription

Values that provide additional information about the transaction amount.

