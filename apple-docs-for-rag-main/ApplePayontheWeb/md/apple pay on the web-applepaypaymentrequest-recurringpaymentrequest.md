

- Apple Pay on the Web
- ApplePayPaymentRequest
-  recurringPaymentRequest 

Instance Property

# recurringPaymentRequest

A property that requests a recurring payment, typically a subscription.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayRecurringPaymentRequest recurringPaymentRequest;
```

## Mentioned in 

Apple Pay on the Web Version 14 Release Notes

## Discussion

This property is optional. Use it to indicate that the payment request is for a recurring payment.

Apple Pay issues an Apple Pay Merchant Token if the user’s payment network supports merchant-specific payment tokens. Otherwise, Apple Pay issues a device token for the payment request.

Important

You can’t use this property with multiTokenContexts or automaticReloadPaymentRequest properties. Simultaneous use of these properties results in an error and cancels the payment request.

## See Also

### Requesting recurring payments

ApplePayRecurringPaymentRequest

A dictionary that represents a request to set up a recurring payment, typically a subscription.

