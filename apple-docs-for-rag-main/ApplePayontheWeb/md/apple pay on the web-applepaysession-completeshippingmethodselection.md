

- Apple Pay on the Web
- ApplePaySession
-  completeShippingMethodSelection 

Instance Method

# completeShippingMethodSelection

Completes the selection of a shipping method with an update.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
undefined completeShippingMethodSelection(
 unsigned short
);
```

## Mentioned in 

Apple Pay on the Web Version 3 Release Notes

## Discussion

This method must be called by onshippingmethodselected.

For Apple Pay JS API version 3, the parameter is an ApplePayShippingMethodUpdate object.

### completeShippingMethodSelection in Apple Pay JS API version 1 and 2

In Apple Pay JS API version 1 and 2, completeShippingMethodSelection has the following parameters:

`status`

The status of the shipping method update. For valid values, see Apple Pay Status Codes. If status is not STATUS_SUCCESS, pass null for the other parameters.

`newTotal`

An ApplePayLineItem dictionary representing the total price for the purchase. Set the label to the merchant’s name, and the amount to the total price. The amount must be greater than zero.

`newLineItems`

A sequence of ApplePayLineItem dictionaries. Use ApplePayLineItem dictionaries to represent all other costs or discounts.

Do not use line items to represent the individual items purchased by the user. Instead, combine all the purchases into a single subtotal item. Use additional line items to represent other costs or discounts (tax, shipping, coupons, and so forth.).

If you do not have any additional costs or discounts, do not use this argument. Set the `newTotal` argument with the total cost of all the purchased items, and either pass an empty array or null for `newLineItems`.

## See Also

### Related Documentation

supportsVersion

Detects whether a web browser supports a particular Apple Pay version.

### Handling shipping method updates

onshippingmethodselected

An event handler to call when the user selects a shipping method.

ApplePayShippingMethodSelectedEvent

An event object that contains the shipping method.

ApplePayShippingMethodUpdate

Updated transaction details that result from a change in shipping method.

