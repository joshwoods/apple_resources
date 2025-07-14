

- Apple Pay on the Web
-  ApplePayPaymentAuthorizationResult 

Structure

# ApplePayPaymentAuthorizationResult

The result of payment authorization, including status and errors.

Safari Desktop 10.0+Safari Mobile 10.0+

**Unsupported OS: Safari Desktop**

``` source
dictionary ApplePayPaymentAuthorizationResult {
 required short status;
 sequence  errors;
 ApplePayPaymentOrderDetails orderDetails;
};
```

**Unsupported OS: Safari Mobile**

``` source
dictionary ApplePayPaymentAuthorizationResult {
 required short status;
 sequence  errors;
 ApplePayPaymentOrderDetails orderDetails;
};
```

## Mentioned in 

Apple Pay on the Web Version 3 Release Notes

## Overview

Use the Apple Pay Status Codes values of STATUS_SUCCESS to indicate when the payment authorization succeeds, or STATUS_FAILURE, along with the errors, when it fails.

## Topics

### Providing authorization results

status

The status code for the authorization result.

errors

A list of custom errors to display on the payment sheet.

### Providing order details

orderDetails

Optional metadata for an order that the customer placed using this payment method.

ApplePayPaymentOrderDetails

A dictionary that contains metadata related to an order.

## See Also

### Handling payment authorization

onpaymentauthorized

An event handler the system calls when the user has authorized the Apple Pay payment with Touch ID, Face ID, or a passcode.

completePayment

Completes the payment authorization with a result.

ApplePayPaymentAuthorizedEvent

An event object that contains the token used to authorize a payment.

ApplePayPayment

The result of authorizing a payment request that contains payment information.

