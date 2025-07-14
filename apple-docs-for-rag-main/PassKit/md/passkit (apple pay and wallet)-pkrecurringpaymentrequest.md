

- PassKit (Apple Pay and Wallet)
-  PKRecurringPaymentRequest 

Class

# PKRecurringPaymentRequest

A class that represents a request to set up a recurring payment, typically a subscription.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class PKRecurringPaymentRequest
```

## Overview

Important

You must set the recurringPaymentRequest property on a PKPaymentRequest object to use this class to request a recurring payment.

Use a PKRecurringPaymentRequest object to provide the user with payment details and a way to manage payment methods for a recurring payment. You can optionally display a billing agreement and set up merchant token life cycle notifications for the request.

For more information about the merchant token life cycle notifications, see Apple Pay Merchant Token Management API.

## Topics

### Creating a recurring payment request

init(paymentDescription: String, regularBilling: PKRecurringPaymentSummaryItem, managementURL: URL)

Create a recurring payment object with a description, regular billing information, and a management URL.

### Describing a recurring payment

var paymentDescription: String

A description that you provide of the recurring payment and that Apple Pay displays to the user in the payment sheet.

var billingAgreement: String?

A localized billing agreement that the payment sheet displays to the user before the user authorizes the payment.

### Setting payment summary items

var regularBilling: PKRecurringPaymentSummaryItem

The regular billing cycle for the recurring payment, including start and end dates, an interval, and an interval count.

var trialBilling: PKRecurringPaymentSummaryItem?

The trial billing cycle for the recurring payment.

class PKRecurringPaymentSummaryItem

An object that defines a summary item for a payment that occurs repeatedly at a specified interval, such as a subscription.

### Managing payment tokens

var tokenNotificationURL: URL?

A URL you provide to receive life-cycle notifications from the Apple Pay servers about the Apple Pay merchant token for the recurring payment.

var managementURL: URL

A URL to a web page where the user can update or delete the payment method for the recurring payment.

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

class PKAutomaticReloadPaymentRequest

A class that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

class PKDeferredPaymentRequest

An object that represents a request to set up a deferred payment, such as a hotel booking or a pre-order.

class PKPaymentTokenContext

A class that defines the context for a single payment token in a payment request for multimerchant payments.

