

- Apple Pay on the Web
- ApplePayShippingContactUpdate
-  newAutomaticReloadPaymentRequest 

Instance Property

# newAutomaticReloadPaymentRequest

An updated request for an automatic reload payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayAutomaticReloadPaymentRequest newAutomaticReloadPaymentRequest;
```

## Discussion

Provide this object to update the automaticReloadPaymentRequest value in the original ApplePayPaymentRequest, if necessary, after the user updated their shipping contact information.

## See Also

### Updating automatic reload payments

ApplePayAutomaticReloadPaymentRequest

A dictionary that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

