

- Apple Pay on the Web
- ApplePaySession
-  onpaymentmethodselected 

Instance Property

# onpaymentmethodselected

An event handler to call when the user selects a new payment method.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute EventHandler onpaymentmethodselected;
```

## Discussion

This attribute must be set to a function that accepts an `events` argument; for example, `session.onpaymentmethodselected = function(event) {}`.

The event parameter contains the paymentMethod attribute. Access it like this:

`var myPaymentMethod = event.paymentMethod;`

The onpaymentmethodselected function must respond by calling completePaymentMethodSelection before the 30 second timeout, after which a message appears stating that the payment could not be completed.

## See Also

### Handling payment method updates

completePaymentMethodSelection

Completes the selection of a payment method with an update.

ApplePayPaymentMethodUpdate

Updated transaction details to provide after the user changes the payment method in the payment sheet.

ApplePayPaymentMethodSelectedEvent

An event object that contains the payment method.

ApplePayPaymentMethod

A dictionary that describes an Apple Pay payment method.

