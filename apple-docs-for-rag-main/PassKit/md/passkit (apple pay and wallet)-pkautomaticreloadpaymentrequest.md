

- PassKit (Apple Pay and Wallet)
-  PKAutomaticReloadPaymentRequest 

Class

# PKAutomaticReloadPaymentRequest

A class that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class PKAutomaticReloadPaymentRequest
```

## Overview

Important

You must set the automaticReloadPaymentRequest property on a PKPaymentRequest object to use the PKAutomaticReloadPaymentRequest class and set up an automatic reload payment.

Apple Pay issues an Apple Pay Merchant Token if the user’s payment network supports merchant-specific payment tokens. Otherwise, Apple Pay issues a device token for the payment request.

Use a PKAutomaticReloadPaymentRequest object to provide the user with payment details and a way to manage payment methods for an automatic reload payment. You can optionally display a billing agreement and set up merchant token life cycle notifications for the request.

## Topics

### Creating an automatic reload payment request

init(paymentDescription: String, automaticReloadBilling: PKAutomaticReloadPaymentSummaryItem, managementURL: URL)

Create an automatic reload payment object with a description, automatic billing information, and a management URL.

### Describing an automatic reload payment

var paymentDescription: String

A description that you provide of the automatic reload payment and that Apple Pay displays to the user in the payment sheet.

var billingAgreement: String?

A localized billing agreement that the payment sheet displays to the user before the user authorizes the payment.

### Setting the payment summary items

var automaticReloadBilling: PKAutomaticReloadPaymentSummaryItem

Summary items that contain the top-up amount and balance threshold amount for the automatic reload payment.

class PKAutomaticReloadPaymentSummaryItem

An object that defines a summary item for an automatic reload or refill payment, such as a store card top-up.

### Managing payment tokens

var managementURL: URL

A URL to a web page where the user can manage and delete the payment method for the automatic reload payment.

var tokenNotificationURL: URL?

A URL you provide to receive life-cycle notifications from the Apple Pay servers about the Apple Pay merchant token for the automatic reload payment.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Payment requests

class PKPaymentRequest

An object that represents a request for payment, including details about payment-processing capabilities, the payment amount, and shipping information.

class PKRecurringPaymentRequest

A class that represents a request to set up a recurring payment, typically a subscription.

class PKDeferredPaymentRequest

An object that represents a request to set up a deferred payment, such as a hotel booking or a pre-order.

class PKPaymentTokenContext

A class that defines the context for a single payment token in a payment request for multimerchant payments.

