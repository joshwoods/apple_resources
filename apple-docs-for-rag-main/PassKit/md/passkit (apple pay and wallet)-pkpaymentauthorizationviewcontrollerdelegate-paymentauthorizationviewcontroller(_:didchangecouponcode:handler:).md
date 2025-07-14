

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewController(\_:didChangeCouponCode:handler:) 

Instance Method

# paymentAuthorizationViewController(\_:didChangeCouponCode:handler:)

Tells the delegate that the user entered or updated a coupon code.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didChangeCouponCode couponCode: String,
    handler completion: @escaping (PKPaymentRequestCouponCodeUpdate) -> Void
)
```

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didChangeCouponCode couponCode: String
) async -> PKPaymentRequestCouponCodeUpdate
```

## Parameters 

`controller`  

The payment authorization view controller.

`couponCode`  

The coupon code.

`completion`  

The completion handler to call with the updated payment summary items and shipping methods.

