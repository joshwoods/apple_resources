

- Apple Pay on the Web
-  ApplePayCouponCodeChangedEvent 

Class

# ApplePayCouponCodeChangedEvent

An event object that contains the coupon code entered by the user.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
interface ApplePayCouponCodeChangedEvent
```

## Mentioned in 

Apple Pay on the Web Version 12 Release Notes

## Topics

### Reading the Coupon Code

couponCode

The updated coupon code from the payment sheet.

## See Also

### Handling coupons

oncouponcodechanged

An event handler called by the system when the user enters or updates a coupon code.

completeCouponCodeChange

Completes the entry of a coupon code with an update.

ApplePayCouponCodeUpdate

A dictionary that contains the updated transaction details for responding to a coupon changed event.

