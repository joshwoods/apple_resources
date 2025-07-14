

- PassKit (Apple Pay and Wallet)
- PKPaymentError
-  PKPaymentError.Code 

Enumeration

# PKPaymentError.Code

An error code that you provide to indicate problems with address or contact information on an Apple Pay sheet.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
enum Code
```

## Overview

The user must resolve any errors that you report on the Apple Pay sheet before they’re able to authorize the transaction. You return any errors in PKPaymentAuthorizationResult or PKPaymentRequestShippingContactUpdate.

You can build your own payment error (NSError), or use one of the following convenience methods from PKPaymentRequest to build it for you.

For an error with contact information: paymentContactInvalidError(withContactField:localizedDescription:).

For a shipping address that is unserviceable: paymentShippingAddressUnserviceableError(withLocalizedDescription:).

For an error with the billing address: paymentBillingAddressInvalidError(withKey:localizedDescription:).

For an error with the shipping address: paymentShippingAddressInvalidError(withKey:localizedDescription:).

The following code example shows:

- How to create a payment error directly.

- How to create a payment error using a convenience method.

Creating payment errors:

```
```

## Topics

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

case unknownError

The error code that indicates an unknown error.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct PKDisbursementError

A structure that describes errors that can occur while processing the disbursement.

struct PKDisbursementErrorKey

Values that describe errors that can occur when processing disbursements.

struct PKPaymentError

An error type that you create to indicate problems with address or contact information on an Apple Pay sheet.

struct PKPaymentErrorKey

Additional details about an error on the Apple Pay sheet.

enum Code

Values that describe errors that can occur while processing the disbursement.

let PKPaymentErrorDomain: String

The error domain for specific errors associated with Apple Pay in-app or web payments.

let PKDisbursementErrorDomain: String

The error domain to use for errors with in-app disbursements.

