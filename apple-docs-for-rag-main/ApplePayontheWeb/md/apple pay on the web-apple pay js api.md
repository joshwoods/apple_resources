

- Apple Pay on the Web
-  Apple Pay JS API 

API Collection

# Apple Pay JS API

Implement Apple Pay on the web using Apple’s JavaScript API.

## Topics

### Apple Pay availability

Checking for Apple Pay availability

Use the Apple Pay JS API to check whether Apple Pay is available, to check whether a device has a payment credential provisioned in Wallet, and to determine when to display an Apple Pay button.

canMakePayments

Indicates whether the device supports Apple Pay.

applePayCapabilities

Indicates whether the device supports Apple Pay and whether the person has an active card in Wallet that qualifies for web payments.

canMakePaymentsWithActiveCard

Indicates whether the device supports Apple Pay and whether the user has an active card in Wallet.

Deprecated

PaymentCredentialStatus

Information about whether the device supports Apple Pay and the possible payment credentials the person has provisioned in Wallet.

PaymentCredentialStatusResponse

The response for information about the device’s support for Apple Pay and the payment credential status.

### Apple Pay payment request

ApplePayPaymentRequest

A request for payment, which includes information about payment-processing capabilities, the payment amount, and shipping information.

ApplePayDeferredPaymentRequest

A dictionary that represents a request to set up a deferred payment, such as a hotel booking or a pre-order.

### Apple Pay session

Creating an Apple Pay Session

Provide a payment request and create the session.

Providing Merchant Validation

Validate your merchant identity and receive a session object for each payment request.

Requesting an Apple Pay payment session

Request a valid session from the Apple Pay server.

ApplePaySession

A session object for managing the payment process on the web.

### Status and errors

ApplePayError

A customizable error type that you create to indicate problems with the address or contact information on an Apple Pay sheet.

ApplePayErrorCode

The error code that indicates whether an error on the payment sheet is for shipping or billing information, or for another kind of error.

ApplePayErrorContactField

Names of the fields in the shipping or billing contact information, used to locate errors in the payment sheet.

Apple Pay Status Codes

Codes used to report the status of an Apple Pay session after a callback.

## See Also

### Apple Pay JavaScript APIs

Choosing an API for Implementing Apple Pay on Your Website

Compare Apple Pay JS and Payment Request API to choose the right implementation for your website.

Apple Pay on the Web version history

Learn about features in each version of Apple Pay on the Web.

Payment Request API

Accept payments on your website with Apple Pay using the Payment Request API.

