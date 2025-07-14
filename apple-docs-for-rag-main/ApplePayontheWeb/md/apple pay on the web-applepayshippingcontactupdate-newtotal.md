

- Apple Pay on the Web
- ApplePayShippingContactUpdate
-  newTotal 

Instance Property

# newTotal

The new total that results from a change in the shipping contact.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required ApplePayLineItem newTotal;
```

## Discussion

Recalculate the total for the payment, because it may change as a result of shipping contact changes. The newTotal value is required.

## See Also

### Updating shipping contact properties

errors

A list of custom errors to display on the payment sheet.

newLineItems

An optional list of updated line items.

newShippingMethods

A list of shipping methods that are available to the updated shipping contact.

