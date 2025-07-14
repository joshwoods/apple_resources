

- Apple Pay on the Web
- ApplePayPaymentMethodUpdate
-  newShippingMethods 

Instance Property

# newShippingMethods

The updated list of available shipping methods that results from the user’s change to the payment method.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
sequence  newShippingMethods;
```

## Discussion

Supply an updated list of shipping methods if the user’s change in the payment method caused any changes in the shipping methods.

## See Also

### Updating payment method properties

newLineItems

An optional list of updated line items for the payment request that results from the user’s change to the payment method.

newTotal

The new total that results from the user’s change to the payment method.

errors

A list of customized errors you provide that results from the user’s change to the payment method.

