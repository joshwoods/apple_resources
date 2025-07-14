

- Apple Pay on the Web
-  ApplePayPayment 

Structure

# ApplePayPayment

The result of authorizing a payment request that contains payment information.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayPayment {
 required ApplePayPaymentToken token;
 ApplePayPaymentContact billingContact;
 ApplePayPaymentContact shippingContact;
};
```

## Mentioned in 

Setting up the payment request API to accept Apple Pay

## Overview

Data in ApplePayPaymentToken is encrypted. Billing and shipping contact data are not encrypted.

## Topics

### Payment token

token

The encrypted information for an authorized payment.

ApplePayPaymentToken

An object that contains the user’s payment credentials.

ApplePayPaymentMethod

A dictionary that describes an Apple Pay payment method.

ApplePayPaymentMethodType

A string that represents the type of the payment method.

ApplePayPaymentPass

A provisioned payment card for Apple Pay payments.

### Billing and shipping contacts

shippingContact

The shipping contact selected by the user for this transaction.

billingContact

The billing contact selected by the user for this transaction.

ApplePayPaymentContact

Contact information fields to use for billing and shipping contact information.

## See Also

### Handling payment authorization

onpaymentauthorized

An event handler the system calls when the user has authorized the Apple Pay payment with Touch ID, Face ID, or a passcode.

completePayment

Completes the payment authorization with a result.

ApplePayPaymentAuthorizedEvent

An event object that contains the token used to authorize a payment.

ApplePayPaymentAuthorizationResult

The result of payment authorization, including status and errors.

