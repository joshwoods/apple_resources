

- ProximityReader
-  PaymentCardVerificationRequest 

Structure

# PaymentCardVerificationRequest

A request to verify details for a contactless payment card.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
struct PaymentCardVerificationRequest
```

## Overview

Create a `PaymentCardVerificationRequest` object to verify details of a person’s payment card before performing a transaction with that card. For example, you might use a verification request to make sure the person’s card supports a specific currency. After creating a request object, pass it to the readPaymentCard(_:) or readPaymentCard(_:vasRequest:stopOnVASResult:) method of your session to read the card details.

## Topics

### Creating the verification request

init(currencyCode: String, for: PaymentCardVerificationRequest.Reason)

Creates a new verification request using the specified currency and reason information.

### Getting the request details

let currencyCode: String

The ISO 4217 code that indicates the currency type.

let verificationReason: PaymentCardVerificationRequest.Reason

The reason you asked to verify someone’s card.

enum Reason

The reason for the verification request.

### Setting the user interface language

var userInterfaceLanguage: Locale.Language?

The language to use when localizing the user interface.

## Relationships

### Conforms To

- Sendable

## See Also

### Payment requests

struct PaymentCardTransactionRequest

A request for a contactless purchase or refund that includes the purchase amount and currency information.

struct PaymentCardReadResult

The result of a payment card read operation.

