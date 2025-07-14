

- Apple Pay on the Web
- ApplePayModifier
-  multiTokenContexts 

Instance Property

# multiTokenContexts

An array of payment token contexts that requests multiple payment tokens to support a multimerchant payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
sequence  multiTokenContexts;
```

## Mentioned in 

Apple Pay on the Web Version 14 Release Notes

## Discussion

Use multitoken contexts to indicate payments for multiple merchants. This modifier is an array of ApplePayPaymentTokenContext objects. The sum of the amount of all the payment token contexts must be less than or equal to the grand total amount of the enclosing payment request. Otherwise, the request results in a runtime error and cancels the payment request.

Important

You can’t use this property with recurringPaymentRequest or automaticReloadPaymentRequest properties. Simultaneous use of these properties results in an error and cancels the payment request.

## See Also

### Updating multitoken or multimerchant payments

ApplePayPaymentTokenContext

A dictionary that defines the context for a single payment token in a payment request for multimerchant payments.

