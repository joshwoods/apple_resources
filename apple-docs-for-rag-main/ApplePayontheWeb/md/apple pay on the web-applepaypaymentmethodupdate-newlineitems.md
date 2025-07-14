

- Apple Pay on the Web
- ApplePayPaymentMethodUpdate
-  newLineItems 

Instance Property

# newLineItems

An optional list of updated line items for the payment request that results from the user’s change to the payment method.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
sequence  newLineItems;
```

## Discussion

Supply an updated list of line items if the user’s change in the payment method caused any changes in the line items.

## See Also

### Updating payment method properties

newTotal

The new total that results from the user’s change to the payment method.

errors

A list of customized errors you provide that results from the user’s change to the payment method.

newShippingMethods

The updated list of available shipping methods that results from the user’s change to the payment method.

