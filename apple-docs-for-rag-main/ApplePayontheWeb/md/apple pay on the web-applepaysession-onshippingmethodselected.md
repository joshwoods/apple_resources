

- Apple Pay on the Web
- ApplePaySession
-  onshippingmethodselected 

Instance Property

# onshippingmethodselected

An event handler to call when the user selects a shipping method.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute EventHandler onshippingmethodselected;
```

## Discussion

This attribute must be set to a function that accepts an `events` argument; for example, `session.onshippingmethodselected = function(event) {}`.

The event parameter contains the shippingMethod attribute.

The onshippingmethodselected function must respond by calling completeShippingMethodSelection before the 30 second timeout, after which a message appears stating that the payment could not be completed.

## See Also

### Handling shipping method updates

completeShippingMethodSelection

Completes the selection of a shipping method with an update.

ApplePayShippingMethodSelectedEvent

An event object that contains the shipping method.

ApplePayShippingMethodUpdate

Updated transaction details that result from a change in shipping method.

