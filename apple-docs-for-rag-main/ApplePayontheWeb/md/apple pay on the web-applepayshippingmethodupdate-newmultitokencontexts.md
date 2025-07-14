

- Apple Pay on the Web
- ApplePayShippingMethodUpdate
-  newMultiTokenContexts 

Instance Property

# newMultiTokenContexts

An array of updated multitoken contexts for a multimerchant payment request.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
sequence  newMultiTokenContexts;
```

## Discussion

Provide this object to update the multiTokenContexts value in the original ApplePayPaymentRequest, if necessary, after the user updated the shipping method.

