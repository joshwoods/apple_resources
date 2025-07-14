

- PassKit (Apple Pay and Wallet)
- PKPaymentError
-  shippingContactInvalidError 

Type Property

# shippingContactInvalidError

The error code to indicate an invalid shipping address, email, phone, or name.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
static var shippingContactInvalidError: PKPaymentError.Code { get }
```

## Discussion

Use this error code if the shipping contact information on the Apple Pay sheet has an error in the address, email, phone, or name.

## See Also

### Identifying the error

static var billingContactInvalidError: PKPaymentError.Code

The error code to indicate an invalid billing address or billing name.

static var shippingAddressUnserviceableError: PKPaymentError.Code

The error code for an unserviceable shipping address.

static var couponCodeExpiredError: PKPaymentError.Code

The error code that indicates an expired coupon.

static var couponCodeInvalidError: PKPaymentError.Code

The error code that indicates an invalid coupon.

static var unknownError: PKPaymentError.Code

The error code for an unknown error.

enum Code

An error code that you provide to indicate problems with address or contact information on an Apple Pay sheet.

