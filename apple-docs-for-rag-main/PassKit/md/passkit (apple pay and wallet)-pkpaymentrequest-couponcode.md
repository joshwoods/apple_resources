

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  couponCode 

Instance Property

# couponCode

The initial coupon code for the payment request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var couponCode: String? { get set }
```

## Discussion

Set the value to `nil` or the empty string to indicate that there’s no initial coupon.

Important

The system doesn’t send a change event for an initial coupon code. You must apply the code to the initial payment summary items.

## See Also

### Working with coupon codes

var supportsCouponCode: Bool

A Boolean value that determines whether the payment sheet displays the coupon code field.

