

- Apple Pay on the Web
- ApplePayPaymentRequest
-  automaticReloadPaymentRequest 

Instance Property

# automaticReloadPaymentRequest

A property that requests an automatic reload payment, such as a store card top-up.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayAutomaticReloadPaymentRequest automaticReloadPaymentRequest;
```

## Mentioned in 

Apple Pay on the Web Version 14 Release Notes

## Discussion

Set this property to indicate that the payment request is for an automatic reload payment.

Apple Pay issues an Apple Pay Merchant Token if the user’s payment network supports merchant-specific payment tokens. Otherwise, Apple Pay issues a device token for the payment request.

Important

You can’t use this property with multiTokenContexts or recurringPaymentRequest properties. Simultaneous use of these properties results in an error and cancels the payment request.

## See Also

### Requesting automatic reload payments

ApplePayAutomaticReloadPaymentRequest

A dictionary that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

