

- Apple Pay on the Web
- ApplePayPaymentMethodUpdate
-  newRecurringPaymentRequest 

Instance Property

# newRecurringPaymentRequest

An updated request for a recurring payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayRecurringPaymentRequest newRecurringPaymentRequest;
```

## Discussion

Provide this object to update the recurringPaymentRequest value in the original ApplePayPaymentRequest, if necessary, after the user updated their payment method.

Important

You can’t use this property with newMultiTokenContexts or newAutomaticReloadPaymentRequest properties. Simultaneous use of these properties results in an error and cancels the payment request.

## See Also

### Updating recurring payments

ApplePayRecurringPaymentRequest

A dictionary that represents a request to set up a recurring payment, typically a subscription.

