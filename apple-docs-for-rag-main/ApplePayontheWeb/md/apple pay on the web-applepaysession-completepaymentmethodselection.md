

- Apple Pay on the Web
- ApplePaySession
-  completePaymentMethodSelection 

Instance Method

# completePaymentMethodSelection

Completes the selection of a payment method with an update.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
undefined completePaymentMethodSelection(
 ApplePayLineItem newTotal,
 sequence newLineItems
);
```

## Mentioned in 

Apple Pay on the Web Version 3 Release Notes

## Discussion

This method must be called by onpaymentmethodselected .

The parameter for the Apple Pay JS API version 3 is an ApplePayPaymentMethodUpdate instance. Use the newLineItems only if you have new or updated costs or discounts, otherwise pass an empty array or null. Set the newTotal argument with the total cost of all the purchased items.

### completePaymentMethodSelection in Apple Pay JS API versions 1 and 2

The parameters for completePaymentMethodSelection in API versions 1 and 2 are:

`newTotal`

An ApplePayLineItem dictionary representing the total price for the purchase. Set the `label` to the merchant’s name, and the `amount` to the total price. The `amount` must be greater than zero.

`newLineItems`

A sequence of ApplePayLineItem dictionaries. Use these line items to represent all other costs or discounts.

Do not use line items to represent the individual items purchased by the user. Instead, combine all the purchases into a single subtotal item. Use additional line items to represent other costs or discounts (tax, shipping, coupons, and so forth.).

## See Also

### Related Documentation

supportsVersion

Detects whether a web browser supports a particular Apple Pay version.

### Handling payment method updates

onpaymentmethodselected

An event handler to call when the user selects a new payment method.

ApplePayPaymentMethodUpdate

Updated transaction details to provide after the user changes the payment method in the payment sheet.

ApplePayPaymentMethodSelectedEvent

An event object that contains the payment method.

ApplePayPaymentMethod

A dictionary that describes an Apple Pay payment method.

