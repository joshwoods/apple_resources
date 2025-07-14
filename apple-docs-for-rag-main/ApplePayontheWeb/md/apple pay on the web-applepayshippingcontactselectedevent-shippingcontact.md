

- Apple Pay on the Web
- ApplePayShippingContactSelectedEvent
-  shippingContact 

Instance Property

# shippingContact

The shipping address selected by the user.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
readonly attribute ApplePayPaymentContact shippingContact;
```

## Discussion

This attribute is contained by the onshippingcontactselected event. Access this attribute using the event parameter in the callback function; for example, `var myShippingContact = event.shippingContact;`.

