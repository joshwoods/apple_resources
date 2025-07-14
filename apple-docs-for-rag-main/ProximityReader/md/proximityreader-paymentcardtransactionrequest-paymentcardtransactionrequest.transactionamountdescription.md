

- ProximityReader
- PaymentCardTransactionRequest
-  PaymentCardTransactionRequest.TransactionAmountDescription 

Enumeration

# PaymentCardTransactionRequest.TransactionAmountDescription

Values that provide additional information about the transaction amount.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
enum TransactionAmountDescription
```

## Overview

This information appears below the central transaction details in the system UI. Each case applies to specific types of transactions, such as a purchase or refund. Check the PaymentCardTransactionRequest.TransactionAmountDescription values description. If an incompatible transaction type is requested or the value(s) are out of range, it will simply not appear in the system UI.

## Topics

### Enumeration Cases

case installment(PaymentCardTransactionRequest.PaymentCycle, amount: Decimal, payments: Int)

The total amount authorized upfront. The customer pays the specified amount on each payment cycle. Only allowed for PaymentCardTransactionRequest.TransactionType.purchase

case membership(PaymentCardTransactionRequest.PaymentCycle)

Charges the customer the amount shown for each payment cycle. Only allowed for PaymentCardTransactionRequest.TransactionType.purchase

case preauthorization

Places a temporary hold on the customer’s account. Only allowed for PaymentCardTransactionRequest.TransactionType.purchase

case preauthorizationAmount(Decimal)

Places a temporary hold on the customer’s account for the specified amount. Only allowed for PaymentCardTransactionRequest.TransactionType.purchase

case preauthorizationRelease

Releases the amount shown from the temporary deposit. Only allowed for PaymentCardTransactionRequest.TransactionType.refund

case surchargeAmount(Decimal)

The transaction’s surcharge amount. Only allowed for PaymentCardTransactionRequest.TransactionType.purchase

case surchargePercent(Double)

The maximum surcharge percentage the payment processor may apply to the transaction. Only allowed for PaymentCardTransactionRequest.TransactionType.purchase

## Relationships

### Conforms To

- Sendable

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

var transactionDescription: PaymentCardTransactionRequest.TransactionAmountDescription?

An optional description of the current transaction meant to provide more context, such as a recurring payment being setup or a surcharge applied.

