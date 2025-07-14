

- PassKit (Apple Pay and Wallet)
- PKPaymentError
-  couponCodeInvalidError 

Type Property

# couponCodeInvalidError

The error code that indicates an invalid coupon.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static var couponCodeInvalidError: PKPaymentError.Code { get }
```

## Discussion

Use this error code if the user entered an invalid coupon code in the payment sheet. You can use paymentCouponCodeInvalidError(localizedDescription:) to create an invalid coupon error object.

Note

A coupon code error doesn’t prevent the user from authorizing the payment.

## See Also

### Identifying the error

static var billingContactInvalidError: PKPaymentError.Code

The error code to indicate an invalid billing address or billing name.

static var shippingContactInvalidError: PKPaymentError.Code

The error code to indicate an invalid shipping address, email, phone, or name.

static var shippingAddressUnserviceableError: PKPaymentError.Code

The error code for an unserviceable shipping address.

static var couponCodeExpiredError: PKPaymentError.Code

The error code that indicates an expired coupon.

static var unknownError: PKPaymentError.Code

The error code for an unknown error.

enum Code

An error code that you provide to indicate problems with address or contact information on an Apple Pay sheet.

