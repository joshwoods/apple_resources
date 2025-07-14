

- Apple Pay on the Web
-  ApplePayPaymentMethodSelectedEvent 

Class

# ApplePayPaymentMethodSelectedEvent

An event object that contains the payment method.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
interface ApplePayPaymentMethodSelectedEvent
```

## Overview

The event handler onpaymentmethodselected receives this event object when the payment method is selected.

## Topics

### Payment method properties

paymentMethod

The card used to complete a payment.

## See Also

### Handling payment method updates

onpaymentmethodselected

An event handler to call when the user selects a new payment method.

completePaymentMethodSelection

Completes the selection of a payment method with an update.

ApplePayPaymentMethodUpdate

Updated transaction details to provide after the user changes the payment method in the payment sheet.

ApplePayPaymentMethod

A dictionary that describes an Apple Pay payment method.

