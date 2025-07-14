

- Apple Pay on the Web
- ApplePayShippingMethodSelectedEvent
-  shippingMethod 

Instance Property

# shippingMethod

The shipping method selected by the user.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
readonly attribute ApplePayShippingMethod shippingMethod;
```

## Discussion

See ApplePayShippingMethod.

This attribute is contained by the onshippingmethodselected event. Access this attribute using the `event` parameter in the callback function; for example, `var myShippingMethod = event.shippingMethod;`.

