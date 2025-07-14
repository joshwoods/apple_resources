

- Apple Pay on the Web
- ApplePayPaymentMethodSelectedEvent
-  paymentMethod 

Instance Property

# paymentMethod

The card used to complete a payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
readonly attribute ApplePayPaymentMethod paymentMethod;
```

## Discussion

See ApplePayPaymentMethod. For privacy reasons, only the `type` property (ApplePayPaymentMethodType) is provided in most cases before the user authorizes the transaction.

This attribute is contained by the onpaymentmethodselected event. Access this attribute using the event parameter in the callback function; for example, `var myPaymentMethod = event.paymentMethod;`.

