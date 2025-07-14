

- PassKit (Apple Pay and Wallet)
-  PKPaymentAuthorizationResult 

Class

# PKPaymentAuthorizationResult

An object that reports the status code and errors for a payment authorization request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class PKPaymentAuthorizationResult
```

## Overview

If the Apple Pay sheet contains errors, you provide a PKPaymentAuthorizationStatus.failure status to PKPaymentAuthorizationResult, and include the errors in the errors array. If there are no errors, you provide a PKPaymentAuthorizationStatus.success status and leave the error array empty.

The following code example shows a failure result with two errors in the postal code and street fields.

A result that reports two errors:

```
// Error in postal code field.
let shippingInvalidZip =
PKPaymentRequest.paymentShippingAddressInvalidError(withKey:CNPostalAddressPostalCodeKey,
                                                    localizedDescription: "Invalid ZIP code")
// Error in street address field.
let shippingInvalidStreet = PKPaymentRequest.paymentShippingAddressInvalidError(withKey:CNPostalAddressStreetKey,
                                                    localizedDescription: "Missing street name")
// Result with failure status and errors.
let result = PKPaymentAuthorizationResult(status: .failure, 
                                          errors: [shippingInvalidZip, shippingInvalidStreet])
```

## Topics

### Initializing a payment authorization result

init(status: PKPaymentAuthorizationStatus, errors: [any Error]?)

Initializes the result with the status code and list of errors.

### Setting order details

var orderDetails: PKPaymentOrderDetails?

Optional metadata with order details for the placed order.

class PKPaymentOrderDetails

Optional metadata with payment order details for the placed order.

### Setting payment authorization status and errors

var errors: [any Error]!

List of errors in the Apple Pay sheet.

var status: PKPaymentAuthorizationStatus

Payment authorization general status.

enum PKPaymentAuthorizationStatus

General success and failure status for payment authorization.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Payment sheet interactions and authorization

class PKPaymentOrderDetails

Optional metadata with payment order details for the placed order.

class PKPaymentAuthorizationController

An object that presents a sheet that prompts the user to authorize a payment request.

class PKPaymentAuthorizationViewController

An object that presents a sheet that prompts the user to authorize a payment request.

class PKPayment

Represents the result of authorizing a payment request and contains payment information, encrypted in the payment token.

