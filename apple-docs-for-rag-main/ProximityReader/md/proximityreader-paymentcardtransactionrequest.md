

- ProximityReader
-  PaymentCardTransactionRequest 

Structure

# PaymentCardTransactionRequest

A request for a contactless purchase or refund that includes the purchase amount and currency information.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
struct PaymentCardTransactionRequest
```

## Mentioned in 

Adding support for Tap to Pay on iPhone to your app

## Overview

Create a `PaymentCardTransactionRequest` to specify the amount of a purchase or refund. After you create this object, pass it to the readPaymentCard(_:) or readPaymentCard(_:vasRequest:stopOnVASResult:) method of PaymentCardReaderSession to read the card associated with the transaction.

## Topics

### Creating a transaction request

init(amount: Decimal, currencyCode: String, for: PaymentCardTransactionRequest.TransactionType)

Creates a new transaction request for the specified amount in the designated currency.

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

enum TransactionAmountDescription

Values that provide additional information about the transaction amount.

### Setting the preferred Application Identifier (AID) list

var preferredAIDList: [Data]

The preferred Application Identifier (AID) or Registered Application Provider Identifier (RID).

### Setting the user interface language

var userInterfaceLanguage: Locale.Language?

The language the framework uses when localizing the user interface.

### Enumerations

enum PaymentCycle

Values that specify the frequency of payments

## Relationships

### Conforms To

- Sendable

## See Also

### Payment requests

struct PaymentCardVerificationRequest

A request to verify details for a contactless payment card.

struct PaymentCardReadResult

The result of a payment card read operation.

