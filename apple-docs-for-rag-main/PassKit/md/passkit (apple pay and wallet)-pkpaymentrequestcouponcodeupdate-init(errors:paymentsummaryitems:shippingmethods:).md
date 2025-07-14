

- PassKit (Apple Pay and Wallet)
- PKPaymentRequestCouponCodeUpdate
-  init(errors:paymentSummaryItems:shippingMethods:) 

Initializer

# init(errors:paymentSummaryItems:shippingMethods:)

Creates a payment coupon update with your specified payment summary items, errors, and shipping methods.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
init(
    errors: [any Error]?,
    paymentSummaryItems: [PKPaymentSummaryItem],
    shippingMethods: [PKShippingMethod]
)
```

## Parameters 

`errors`  

An array of errors for the coupon code that the user must resolve.

`paymentSummaryItems`  

An array of summary items that include any changes due to the coupon.

`shippingMethods`  

An array of shipping methods.

