

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationControllerDelegate
-  paymentAuthorizationController(\_:didChangeCouponCode:handler:) 

Instance Method

# paymentAuthorizationController(\_:didChangeCouponCode:handler:)

Tells the delegate that the user entered or updated a coupon code.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didChangeCouponCode couponCode: String,
    handler completion: @escaping (PKPaymentRequestCouponCodeUpdate) -> Void
)
```

``` source
@MainActor
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didChangeCouponCode couponCode: String
) async -> PKPaymentRequestCouponCodeUpdate
```

## Parameters 

`controller`  

The payment authorization controller.

`couponCode`  

The new coupon code.

`completion`  

The completion handler to call with the updated payment summary items and shipping methods.

