

- Apple Pay on the Web
- ApplePaySession
-  onpaymentauthorized 

Instance Property

# onpaymentauthorized

An event handler the system calls when the user has authorized the Apple Pay payment with Touch ID, Face ID, or a passcode.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute EventHandler onpaymentauthorized;
```

## Discussion

This attribute must be set to a function that accepts an `events` argument; for example, `session.onpaymentauthorized = function(event) {}`.

The event parameter contains the payment (ApplePayPayment) attribute.

The onpaymentauthorized function must complete the payment and respond by calling completePayment before the 30 second timeout, after which a message appears stating that the payment couldn’t be completed.

## See Also

### Handling payment authorization

completePayment

Completes the payment authorization with a result.

ApplePayPaymentAuthorizedEvent

An event object that contains the token used to authorize a payment.

ApplePayPayment

The result of authorizing a payment request that contains payment information.

ApplePayPaymentAuthorizationResult

The result of payment authorization, including status and errors.

