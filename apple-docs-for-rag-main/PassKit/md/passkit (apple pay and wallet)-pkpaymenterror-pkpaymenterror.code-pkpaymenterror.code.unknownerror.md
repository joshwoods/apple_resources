

- PassKit (Apple Pay and Wallet)
- PKPaymentError
- PKPaymentError.Code
-  PKPaymentError.Code.unknownError 

Case

# PKPaymentError.Code.unknownError

The error code that indicates an unknown error.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
case unknownError
```

## Discussion

User this error code if an unknown but non-fatal error occurred during payment processing. The user can attempt to authorize the transaction again.

## See Also

### Error codes

case couponCodeExpiredError

The error code that indicates an expired coupon.

case couponCodeInvalidError

The error code that indicates an invalid coupon.

case billingContactInvalidError

The error code that indicates an invalid billing address or billing name.

case shippingContactInvalidError

The error code that indicates an invalid shipping address, email, phone, or name.

case shippingAddressUnserviceableError

The error code that indicates an unserviceable shipping address.

