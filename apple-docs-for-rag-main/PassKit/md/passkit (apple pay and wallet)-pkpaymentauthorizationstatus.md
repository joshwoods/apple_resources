

- PassKit (Apple Pay and Wallet)
-  PKPaymentAuthorizationStatus 

Enumeration

# PKPaymentAuthorizationStatus

General success and failure status for payment authorization.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
enum PKPaymentAuthorizationStatus
```

## Overview

You pass the payment authorization status along with related errors, if any, to the completion block in PKPaymentAuthorizationResult.

Use the PIN status constants only when working in a region that requires 6-digit PIN numbers. To authorize a payment, follow this workflow:

1.  The app sets up the payment request and displays the authorization view controller.

2.  The user authorizes the payment.

3.  If the purchase amount exceeds the user’s PIN limit or if the purchase uses a currency code other than the one expected by the bank, Apple Pay prompts the user for their PIN.

4.  The user enters their PIN.

5.  Apple Pay calls the delegate’s paymentAuthorizationViewController(_:didAuthorizePayment:completion:) method.

6.  The app either processes the payment or uses a third-party SDK to process the payment. During this step, the PIN number is passed to the bank as part of the PKPaymentToken object.

7.  As soon as the payment is processed, the app calls the completion block, passing the appropriate PKPaymentAuthorizationStatus constant. If the bank reports a problem with the PIN, use the corresponding PIN status constant.

For more information on PIN requirements, check with your payment processor.

## Topics

### Payment authorization status constants

case success

Merchant successfully authorized the transaction, or the transaction is expected to succeed.

case failure

Merchant failed to authorize the transaction.

case invalidBillingPostalAddress

Invalid or unusable billing address.

Deprecated

case invalidShippingPostalAddress

Invalid or unusable shipping address.

Deprecated

case invalidShippingContact

Invalid or incomplete shipping contact.

Deprecated

case pinRequired

Transaction requires PIN entry.

case pinIncorrect

Incorrect PIN entered.

case pinLockout

PIN retry limit exceeded.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting payment authorization status and errors

var errors: [any Error]!

List of errors in the Apple Pay sheet.

var status: PKPaymentAuthorizationStatus

Payment authorization general status.

