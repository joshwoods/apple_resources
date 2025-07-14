

- PassKit (Apple Pay and Wallet)
-  Apple Pay 

API Collection

# Apple Pay

Request and process Apple Pay payments in your app.

## Topics

### Apple Pay setup

Setting up Apple Pay

Fulfill the requirements to provide Apple Pay as a payment option on your website or in your app.

Offering Apple Pay in Your App

Collect payments with iPhone and Apple Watch using Apple Pay.

Complying with regional regulations

Check regional regulations for possible requirements for your Apple Pay-based implementation.

### Apple Pay availability

Determine if the device supports Apple Pay and whether the user has added payment cards.

class PKPaymentAuthorizationController

An object that presents a sheet that prompts the user to authorize a payment request.

class PKPaymentAuthorizationViewController

An object that presents a sheet that prompts the user to authorize a payment request.

### Apple Pay buttons

class PKPaymentButton

An object that displays a button either to trigger payments through Apple Pay or to prompt the user to set up a card.

struct PayWithApplePayButton

struct PayWithApplePayButtonLabel

struct PayWithApplePayButtonStyle

### Payment requests

class PKPaymentRequest

An object that represents a request for payment, including details about payment-processing capabilities, the payment amount, and shipping information.

class PKRecurringPaymentRequest

A class that represents a request to set up a recurring payment, typically a subscription.

class PKAutomaticReloadPaymentRequest

A class that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

class PKDeferredPaymentRequest

An object that represents a request to set up a deferred payment, such as a hotel booking or a pre-order.

class PKPaymentTokenContext

A class that defines the context for a single payment token in a payment request for multimerchant payments.

### Disbursement requests

class PKDisbursementRequest

An object that represents a request to disburse funds from a merchant to an individual.

### Payment sheet interactions and authorization

class PKPaymentAuthorizationResult

An object that reports the status code and errors for a payment authorization request.

class PKPaymentOrderDetails

Optional metadata with payment order details for the placed order.

class PKPaymentAuthorizationController

An object that presents a sheet that prompts the user to authorize a payment request.

class PKPaymentAuthorizationViewController

An object that presents a sheet that prompts the user to authorize a payment request.

class PKPayment

Represents the result of authorizing a payment request and contains payment information, encrypted in the payment token.

### Payment sheet updates

Process the user’s changes and update the payment sheet.

class PKPaymentRequestMerchantSessionUpdate

An object that updates a payment request with a merchant validation.

class PKPaymentRequestPaymentMethodUpdate

An object that updates the payment request after the payment method changes.

class PKPaymentRequestShippingContactUpdate

An object that updates the payment request after the shipping contact information changes.

class PKPaymentRequestShippingMethodUpdate

An object that updates the payment request after the shipping method changed.

class PKPaymentRequestCouponCodeUpdate

An object that updates the payment request after the coupon code changes.

class PKPaymentRequestUpdate

The base class for updating the payment request after the user makes changes on the payment sheet.

### QR transaction information

class PKPaymentInformationEventExtension

An abstract superclass for an extension to collect payment information and sign transaction data in a QR code purchase.

protocol PKPaymentInformationRequestHandling

### Entitlements

Merchant IDs Entitlement

A list of merchant IDs your app uses for Apple Pay support.

### Payment token format

Payment token format reference

Verify an Apple Pay payment token and validate a transaction.

### Errors

Provide granular error information for contact and address data.

struct PKDisbursementError

A structure that describes errors that can occur while processing the disbursement.

struct PKDisbursementErrorKey

Values that describe errors that can occur when processing disbursements.

struct PKPaymentError

An error type that you create to indicate problems with address or contact information on an Apple Pay sheet.

enum Code

An error code that you provide to indicate problems with address or contact information on an Apple Pay sheet.

struct PKPaymentErrorKey

Additional details about an error on the Apple Pay sheet.

enum Code

Values that describe errors that can occur while processing the disbursement.

let PKPaymentErrorDomain: String

The error domain for specific errors associated with Apple Pay in-app or web payments.

let PKDisbursementErrorDomain: String

The error domain to use for errors with in-app disbursements.

### Deprecated

var applePayLaterAvailability: PKPaymentRequest.ApplePayLaterAvailability

A value that indicates whether Apple Pay Later is available for a transaction.

Deprecated

enum ApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Deprecated

struct PKAddressField

Billing or shipping address fields.

Deprecated

enum PKApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Deprecated

## See Also

### Related Documentation

Apple Pay Programming Guide

iOS Human Interface Guidelines

