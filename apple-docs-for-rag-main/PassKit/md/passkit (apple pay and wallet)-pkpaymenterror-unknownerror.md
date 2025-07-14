

- PassKit (Apple Pay and Wallet)
- PKPaymentError
-  unknownError 

Type Property

# unknownError

The error code for an unknown error.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
static var unknownError: PKPaymentError.Code { get }
```

## Discussion

Use this error code if an unknown but non-fatal error occurred during payment processing. The user can attempt authorization again.

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

static var couponCodeInvalidError: PKPaymentError.Code

The error code that indicates an invalid coupon.

enum Code

An error code that you provide to indicate problems with address or contact information on an Apple Pay sheet.

