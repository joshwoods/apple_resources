

- ProximityReader
-  PaymentCardReadResult 

Structure

# PaymentCardReadResult

The result of a payment card read operation.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
struct PaymentCardReadResult
```

## Mentioned in 

Adding support for Tap to Pay on iPhone to your app

Accepting loyalty passes from Wallet

## Overview

The system returns a `PaymentCardReadResult` in response to your requests to read a person’s payment card. Use this information to facilitate payments with your payment service provider.

For information about how to read a payment card, see PaymentCardReaderSession.

## Topics

### Getting the result data

let generalCardData: String?

A Base64-encoded string that contains general cardholder and terminal data in tag-length-value (TLV) format.

let paymentCardData: String?

A Base64-encoded string that contains the encrypted payment information to send to your payment provider.

### Checking the read outcome

let outcome: PaymentCardReadResult.ReadOutcome

The outcome of the transaction.

enum ReadOutcome

Values that describe the outcome of a read request.

### Getting the result ID

let id: String

The unique identifier for the transaction.

### Getting the PIN status

let isPINFallback: Bool

A Boolean value that indicates whether the PIN Fallback occurred.

let pinBypassed: Bool

A Boolean value that indicates whether the consumer bypassed the PIN entry.

### Getting the kernel type

let applicationTypeIdentifier: String?

A string identifier that represents the payment application type (kernel) used to read the card.

### Instance Properties

let cardEffectiveState: PaymentCardReadResult.CardEffectiveState?

The effective state of the card that the system read.

let cardExpirationState: PaymentCardReadResult.CardExpirationState?

The expiration state of the card that the system read.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Enumerations

enum CardEffectiveState

Values that describe the effective state of the card that was read.

enum CardExpirationState

Values that describe the expiration state of the card that the system read.

## Relationships

### Conforms To

- Identifiable
- Sendable

## See Also

### Payment requests

struct PaymentCardTransactionRequest

A request for a contactless purchase or refund that includes the purchase amount and currency information.

struct PaymentCardVerificationRequest

A request to verify details for a contactless payment card.

