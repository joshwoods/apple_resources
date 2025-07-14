

- Apple Pay on the Web
- ApplePayShippingMethodUpdate
-  newTotal 

Instance Property

# newTotal

The new total that results from a change in the shipping method.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required ApplePayLineItem newTotal;
```

## Discussion

Recalculate the total for the payment, because it may change as a result of shipping method changes. The newTotal value is required.

## See Also

### Updating shipping method properties

newLineItems

An optional list of updated line items.

newShippingMethods

An updated list of new shipping methods.

