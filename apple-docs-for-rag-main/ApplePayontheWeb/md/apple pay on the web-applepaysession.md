

- Apple Pay on the Web
-  ApplePaySession 

Class

# ApplePaySession

A session object for managing the payment process on the web.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
interface ApplePaySession
```

## Mentioned in 

Creating an Apple Pay Session

## Overview

ApplePaySession is the entry point for Apple Pay on the web. All the steps of the payment process for a single transaction occur in a session.

ApplePaySession belongs to the Apple Pay JS API.

## Topics

### Determining support for API and payments

supportsVersion

Detects whether a web browser supports a particular Apple Pay version.

applePayCapabilities

Indicates whether the device supports Apple Pay and whether the person has an active card in Wallet that qualifies for web payments.

canMakePayments

Indicates whether the device supports Apple Pay.

canMakePaymentsWithActiveCard

Indicates whether the device supports Apple Pay and whether the user has an active card in Wallet.

Deprecated

### Creating an Apple Pay session

ApplePaySession

The entry point for Apple Pay on the web.

### Getting merchant validation

begin

Begins the merchant validation process.

onvalidatemerchant

An event handler the system calls when it displays the payment sheet.

completeMerchantValidation

Completes the validation for a merchant session.

ApplePayValidateMerchantEvent

An event object that contains the validation URL.

### Handling payment method updates

onpaymentmethodselected

An event handler to call when the user selects a new payment method.

completePaymentMethodSelection

Completes the selection of a payment method with an update.

ApplePayPaymentMethodUpdate

Updated transaction details to provide after the user changes the payment method in the payment sheet.

ApplePayPaymentMethodSelectedEvent

An event object that contains the payment method.

ApplePayPaymentMethod

A dictionary that describes an Apple Pay payment method.

### Handling coupons

oncouponcodechanged

An event handler called by the system when the user enters or updates a coupon code.

completeCouponCodeChange

Completes the entry of a coupon code with an update.

ApplePayCouponCodeChangedEvent

An event object that contains the coupon code entered by the user.

ApplePayCouponCodeUpdate

A dictionary that contains the updated transaction details for responding to a coupon changed event.

### Handling shipping contact updates

onshippingcontactselected

An event handler to call when the user selects a shipping contact in the payment sheet.

completeShippingContactSelection

Completes the selection of a shipping contact with an update.

ApplePayShippingContactSelectedEvent

An event object that contains the shipping address the user selects.

ApplePayShippingContactUpdate

Updated transaction details that result from a change in shipping contact, including any errors.

### Handling shipping method updates

onshippingmethodselected

An event handler to call when the user selects a shipping method.

completeShippingMethodSelection

Completes the selection of a shipping method with an update.

ApplePayShippingMethodSelectedEvent

An event object that contains the shipping method.

ApplePayShippingMethodUpdate

Updated transaction details that result from a change in shipping method.

### Handling payment authorization

onpaymentauthorized

An event handler the system calls when the user has authorized the Apple Pay payment with Touch ID, Face ID, or a passcode.

completePayment

Completes the payment authorization with a result.

ApplePayPaymentAuthorizedEvent

An event object that contains the token used to authorize a payment.

ApplePayPayment

The result of authorizing a payment request that contains payment information.

ApplePayPaymentAuthorizationResult

The result of payment authorization, including status and errors.

### Ending the session

oncancel

An event handler that is automatically called when the payment UI is dismissed.

abort

Aborts the current Apple Pay session.

### Displaying an Apple Pay setup button

openPaymentSetup

A method that displays the Set up Apple Pay button.

### Status code constants

STATUS_FAILURE

The requested action failed.

STATUS_INVALID_BILLING_POSTAL_ADDRESS

The billing address is invalid.

STATUS_INVALID_SHIPPING_CONTACT

The shipping contact information is invalid.

STATUS_INVALID_SHIPPING_POSTAL_ADDRESS

The shipping address is invalid.

STATUS_PIN_INCORRECT

The PIN information is not valid.

STATUS_PIN_LOCKOUT

The maximum number of tries for a PIN has been reached and the user has been locked out.

STATUS_PIN_REQUIRED

The required PIN information was not provided.

STATUS_SUCCESS

The requested action succeeded.

## See Also

### Apple Pay session

Creating an Apple Pay Session

Provide a payment request and create the session.

Providing Merchant Validation

Validate your merchant identity and receive a session object for each payment request.

Requesting an Apple Pay payment session

Request a valid session from the Apple Pay server.

