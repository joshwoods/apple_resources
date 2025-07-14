

- Apple Pay on the Web
- ApplePayPaymentMethodUpdate
-  newMultiTokenContexts 

Instance Property

# newMultiTokenContexts

An array of updated multitoken contexts for a multimerchant payment request.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
sequence  newMultiTokenContexts;
```

## Discussion

Provide this object to update the multiTokenContexts value in the original ApplePayPaymentRequest, if necessary, after the user updated their payment method.

Important

You can’t use this property with newAutomaticReloadPaymentRequest or newRecurringPaymentRequest properties. Simultaneous use of these properties results in an error and cancels the payment request.

## See Also

### Updating multitoken or multimerchant payments

ApplePayPaymentTokenContext

A dictionary that defines the context for a single payment token in a payment request for multimerchant payments.

