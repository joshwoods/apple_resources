

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  supportsCouponCode 

Instance Property

# supportsCouponCode

A Boolean value that determines whether the payment sheet displays the coupon code field.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var supportsCouponCode: Bool { get set }
```

## Discussion

Set the value to `true` to display the coupon code field.

## See Also

### Working with coupon codes

var couponCode: String?

The initial coupon code for the payment request.

