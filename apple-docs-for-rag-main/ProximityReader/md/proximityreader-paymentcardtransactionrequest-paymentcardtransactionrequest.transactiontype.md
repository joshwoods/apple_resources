

- ProximityReader
- PaymentCardTransactionRequest
-  PaymentCardTransactionRequest.TransactionType 

Enumeration

# PaymentCardTransactionRequest.TransactionType

The type of transaction to perform.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
enum TransactionType
```

## Topics

### Getting the transaction type

case purchase

A purchase transaction.

case refund

A refund transaction.

### Operators

static func == (PaymentCardTransactionRequest.TransactionType, PaymentCardTransactionRequest.TransactionType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the transaction details

let amount: Decimal

The amount of the purchase or refund in the specified currency.

let currencyCode: String

The ISO 4217 code that indicates the currency type.

let type: PaymentCardTransactionRequest.TransactionType

The type of transaction, either a purchase or a refund.

var transactionDescription: PaymentCardTransactionRequest.TransactionAmountDescription?

An optional description of the current transaction meant to provide more context, such as a recurring payment being setup or a surcharge applied.

enum TransactionAmountDescription

Values that provide additional information about the transaction amount.

