

- Apple Pay on the Web
- ApplePayPaymentAuthorizedEvent
-  payment 

Instance Property

# payment

The authorized payment information for this transaction.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
readonly attribute ApplePayPayment payment;
```

## Discussion

This attribute is contained by the onpaymentauthorized event. Access this attribute using the event parameter in the callback function; for example, `var payinfo = event.payment;`.

ApplePayPayment contains `billingContact` and `shippingContact` if they were requested, and it also contains ApplePayPaymentToken.

