

- PassKit (Apple Pay and Wallet)
-  PKPaymentError 

Structure

# PKPaymentError

An error type that you create to indicate problems with address or contact information on an Apple Pay sheet.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
struct PKPaymentError
```

## Overview

The user must resolve any errors that you report on the Apple Pay sheet before they’re able to authorize the transaction. You return any errors in PKPaymentAuthorizationResult or PKPaymentRequestShippingContactUpdate.

You can build your own payment error (NSError), or use one of the following convenience methods from PKPaymentRequest to build it for you.

- For an error with contact information, use paymentContactInvalidError(withContactField:localizedDescription:).

- For a shipping address that is unserviceable, use paymentShippingAddressUnserviceableError(withLocalizedDescription:).

- For an error with the billing address, use paymentBillingAddressInvalidError(withKey:localizedDescription:).

- For an error with the shipping address, use paymentShippingAddressInvalidError(withKey:localizedDescription:).

The following code example shows:

- How to create an error directly.

- How to create an error using a convenience method.

Creating payment errors:

```
// A general billing address error created with NSError
let billingAddressError = NSError.init(domain: PKPaymentErrorDomain,
                          code: PKPaymentError.billingContactInvalidError.rawValue,
                          userInfo: [NSLocalizedDescriptionKey:"Address has an error",
                          PKPaymentErrorKey.contactFieldUserInfoKey: PKContactField.postalAddress])

// A specific billing address error created with a convenience method
let billingAddressInvalidStreet = PKPaymentRequest.paymentBillingAddressInvalidError(withKey:CNPostalAddressStreetKey,
                                                   localizedDescription: "Invalid street")
```

## Topics

### Creating a payment error object

init(Code, userInfo: [String : Any])

Creates a payment error object of the specified type with the specified user information.

### Describing the error

var code: Code

The error code for this instance.

var errorCode: Int

The error code for this instance.

var userInfo: [String : Any]

Additional details about the error.

var errorUserInfo: [String : Any]

Additional details about the error.

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

static var unknownError: PKPaymentError.Code

The error code for an unknown error.

enum Code

An error code that you provide to indicate problems with address or contact information on an Apple Pay sheet.

### Querying the error domain

let PKPaymentErrorDomain: String

The error domain for specific errors associated with Apple Pay in-app or web payments.

### Comparing errors

static func == (PKPaymentError, PKPaymentError) -> Bool

Returns a Boolean value indicating whether two payment error objects are equal.

### Hashing

func hash(into: inout Hasher)

Hashes the payment error object by feeding the item into the given hasher.

var hashValue: Int

The hash value for the payment error.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

struct PKDisbursementError

A structure that describes errors that can occur while processing the disbursement.

struct PKDisbursementErrorKey

Values that describe errors that can occur when processing disbursements.

enum Code

An error code that you provide to indicate problems with address or contact information on an Apple Pay sheet.

struct PKPaymentErrorKey

Additional details about an error on the Apple Pay sheet.

enum Code

Values that describe errors that can occur while processing the disbursement.

let PKPaymentErrorDomain: String

The error domain for specific errors associated with Apple Pay in-app or web payments.

let PKDisbursementErrorDomain: String

The error domain to use for errors with in-app disbursements.

