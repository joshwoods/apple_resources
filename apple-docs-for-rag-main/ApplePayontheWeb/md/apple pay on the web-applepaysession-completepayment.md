

- Apple Pay on the Web
- ApplePaySession
-  completePayment 

Instance Method

# completePayment

Completes the payment authorization with a result.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
undefined completePayment();
```

## Parameters 

`result`  

The result of the payment authorization, including its status and list of errors. See ApplePayPaymentAuthorizationResult.

## Mentioned in 

Apple Pay on the Web Version 3 Release Notes

## Discussion

This method must be called by onpaymentauthorized.

Use status values of STATUS_SUCCESS or STATUS_FAILURE only. You should pass in STATUS_FAILURE along with the errors.

### completePayment in Apple Pay JS API version 1 and 2

The parameter for completePayment in versions 1 and 2 is the following:

`status`

The status of the payment, whether it succeeded or failed. See Apple Pay Status Codes.

The Apple Pay payment sheet is dismissed when this method is called with a status value of STATUS_SUCCESS or STATUS_FAILURE. Other status values display an error on the payment sheet to prompt the user to update the information and authenticate again.

## See Also

### Related Documentation

supportsVersion

Detects whether a web browser supports a particular Apple Pay version.

### Handling payment authorization

onpaymentauthorized

An event handler the system calls when the user has authorized the Apple Pay payment with Touch ID, Face ID, or a passcode.

ApplePayPaymentAuthorizedEvent

An event object that contains the token used to authorize a payment.

ApplePayPayment

The result of authorizing a payment request that contains payment information.

ApplePayPaymentAuthorizationResult

The result of payment authorization, including status and errors.

