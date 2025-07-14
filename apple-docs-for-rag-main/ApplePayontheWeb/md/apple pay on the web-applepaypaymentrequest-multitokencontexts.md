

- Apple Pay on the Web
- ApplePayPaymentRequest
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

Use multitoken contexts to indicate payments for multiple merchants. The sum of the amount of all the payment token contexts must be less than or equal to the grand total amount of the enclosing payment request. Otherwise, the request results in an error and cancels the payment request.

Important

You can’t use this array with recurringPaymentRequest or automaticReloadPaymentRequest properties. Simultaneous use of these properties results in an error and cancels the payment request.

## See Also

### Requesting multitoken or multimerchant payments

ApplePayPaymentTokenContext

A dictionary that defines the context for a single payment token in a payment request for multimerchant payments.

