

- Apple Pay on the Web
- ApplePaySession
-  completeCouponCodeChange 

Instance Method

# completeCouponCodeChange

Completes the entry of a coupon code with an update.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
undefined completeCouponCodeChange(
 ApplePayCouponCodeUpdate update
);
```

## Mentioned in 

Apple Pay on the Web Version 12 Release Notes

## Discussion

This is the method called by oncouponcodechanged to complete the event.

## See Also

### Handling coupons

oncouponcodechanged

An event handler called by the system when the user enters or updates a coupon code.

ApplePayCouponCodeChangedEvent

An event object that contains the coupon code entered by the user.

ApplePayCouponCodeUpdate

A dictionary that contains the updated transaction details for responding to a coupon changed event.

