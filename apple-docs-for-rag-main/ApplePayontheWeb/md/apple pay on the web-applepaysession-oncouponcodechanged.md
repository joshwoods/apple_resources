

- Apple Pay on the Web
- ApplePaySession
-  oncouponcodechanged 

Instance Property

# oncouponcodechanged

An event handler called by the system when the user enters or updates a coupon code.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute EventHandler oncouponcodechanged;
```

## Discussion

Set this attribute to a function with one parameter that contains an ApplePayCouponCodeChangedEvent. This function processes the coupon code update, and then calls completeCouponCodeChange with the results.

The code below shows adding a listener for the coupon code changed event to the Apple Pay session:

```
// Add a listener for the couponcodechanged event to the Apple Pay session.
session.addEventListener("couponcodechanged", function(event) {
    var newCode = event.couponCode;

    // Process the coupon code.
    ...

    // Call the Apple Pay session completion method for this event.
    session.completeCouponCodeChange({
        // Update the payment request with any changed information.
        newTotal: ...
    });
});
```

Note

Call `completeCouponCodeChange` within `30` seconds to prevent the system ending the payment request.

## See Also

### Handling coupons

completeCouponCodeChange

Completes the entry of a coupon code with an update.

ApplePayCouponCodeChangedEvent

An event object that contains the coupon code entered by the user.

ApplePayCouponCodeUpdate

A dictionary that contains the updated transaction details for responding to a coupon changed event.

