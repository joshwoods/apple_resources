

- Apple Pay on the Web
-  ApplePayPaymentAuthorizedEvent 

Class

# ApplePayPaymentAuthorizedEvent

An event object that contains the token used to authorize a payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
interface ApplePayPaymentAuthorizedEvent
```

## Overview

The event handler onpaymentauthorized receives this event object when a payment is authorized.

## Topics

### Payment property

payment

The authorized payment information for this transaction.

## See Also

### Handling payment authorization

onpaymentauthorized

An event handler the system calls when the user has authorized the Apple Pay payment with Touch ID, Face ID, or a passcode.

completePayment

Completes the payment authorization with a result.

ApplePayPayment

The result of authorizing a payment request that contains payment information.

ApplePayPaymentAuthorizationResult

The result of payment authorization, including status and errors.

