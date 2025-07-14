

- Apple Pay on the Web
- ApplePayCouponCodeUpdate
-  newAutomaticReloadPaymentRequest 

Instance Property

# newAutomaticReloadPaymentRequest

An updated request for an automatic reload payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayAutomaticReloadPaymentRequest newAutomaticReloadPaymentRequest;
```

## Discussion

Provide this object to update the automaticReloadPaymentRequest value in the original ApplePayPaymentRequest, if necessary, after the user updated the coupon code.

