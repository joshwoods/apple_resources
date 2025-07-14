

- Apple Pay on the Web
- ApplePayRequestBase
-  couponCode 

Instance Property

# couponCode

The initial coupon code for the payment request.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
DOMString couponCode;
```

## Discussion

Set the value to `nil` or the empty string to indicate that there’s no initial coupon.

Important

The system doesn’t send a change event for an initial coupon code. You must apply the code to the initial payment summary items.

## See Also

### Managing coupon codes

supportsCouponCode

A Boolean value that determines whether the payment sheet displays the coupon code field.

