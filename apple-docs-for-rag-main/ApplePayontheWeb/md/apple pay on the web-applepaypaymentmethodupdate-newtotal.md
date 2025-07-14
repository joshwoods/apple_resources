

- Apple Pay on the Web
- ApplePayPaymentMethodUpdate
-  newTotal 

Instance Property

# newTotal

The new total that results from the user’s change to the payment method.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required ApplePayLineItem newTotal;
```

## Discussion

Calculate the total for the payment, as it may change after the user updated the payment method. This value is required.

## See Also

### Updating payment method properties

newLineItems

An optional list of updated line items for the payment request that results from the user’s change to the payment method.

errors

A list of customized errors you provide that results from the user’s change to the payment method.

newShippingMethods

The updated list of available shipping methods that results from the user’s change to the payment method.

