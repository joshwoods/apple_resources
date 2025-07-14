

- PassKit (Apple Pay and Wallet)
- PKPaymentError
- PKPaymentError.Code
-  PKPaymentError.Code.billingContactInvalidError 

Case

# PKPaymentError.Code.billingContactInvalidError

The error code that indicates an invalid billing address or billing name.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
case billingContactInvalidError
```

## Discussion

Use this error code if the billing contact information on the Apple Pay sheet has an error in the address or name.

## See Also

### Error codes

case couponCodeExpiredError

The error code that indicates an expired coupon.

case couponCodeInvalidError

The error code that indicates an invalid coupon.

case shippingContactInvalidError

The error code that indicates an invalid shipping address, email, phone, or name.

case shippingAddressUnserviceableError

The error code that indicates an unserviceable shipping address.

case unknownError

The error code that indicates an unknown error.

