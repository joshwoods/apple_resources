

- ProximityReader
- PaymentCardTransactionRequest
-  type 

Instance Property

# type

The type of transaction, either a purchase or a refund.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
let type: PaymentCardTransactionRequest.TransactionType
```

## See Also

### Getting the transaction details

let amount: Decimal

The amount of the purchase or refund in the specified currency.

let currencyCode: String

The ISO 4217 code that indicates the currency type.

enum TransactionType

The type of transaction to perform.

var transactionDescription: PaymentCardTransactionRequest.TransactionAmountDescription?

An optional description of the current transaction meant to provide more context, such as a recurring payment being setup or a surcharge applied.

enum TransactionAmountDescription

Values that provide additional information about the transaction amount.

