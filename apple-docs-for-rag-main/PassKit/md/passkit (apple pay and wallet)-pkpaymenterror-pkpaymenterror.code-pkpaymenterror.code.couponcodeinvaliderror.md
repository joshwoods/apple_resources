

- PassKit (Apple Pay and Wallet)
- PKPaymentError
- PKPaymentError.Code
-  PKPaymentError.Code.couponCodeInvalidError 

Case

# PKPaymentError.Code.couponCodeInvalidError

The error code that indicates an invalid coupon.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
case couponCodeInvalidError
```

## Discussion

Use this error code if the coupon code entered in the payment sheet is invalid. You can use paymentCouponCodeInvalidError(localizedDescription:) to create an expired coupon error object.

## See Also

### Error codes

case couponCodeExpiredError

The error code that indicates an expired coupon.

case billingContactInvalidError

The error code that indicates an invalid billing address or billing name.

case shippingContactInvalidError

The error code that indicates an invalid shipping address, email, phone, or name.

case shippingAddressUnserviceableError

The error code that indicates an unserviceable shipping address.

case unknownError

The error code that indicates an unknown error.

