

- PassKit (Apple Pay and Wallet)
- PKPaymentError
- PKPaymentError.Code
-  PKPaymentError.Code.shippingAddressUnserviceableError 

Case

# PKPaymentError.Code.shippingAddressUnserviceableError

The error code that indicates an unserviceable shipping address.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
case shippingAddressUnserviceableError
```

## Discussion

Use this error code for a shipping address that is otherwise valid, but is unserviceable. For example, the address is in a country or region you don’t ship to, or it’s a P.O. box and you can’t deliver to P.O. boxes.

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

case unknownError

The error code that indicates an unknown error.

