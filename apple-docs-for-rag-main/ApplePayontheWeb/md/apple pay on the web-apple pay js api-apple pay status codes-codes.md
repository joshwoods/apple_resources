

- Apple Pay on the Web
- Apple Pay JS API
-  Apple Pay Status Codes 

API Collection

# Apple Pay Status Codes

Codes used to report the status of an Apple Pay session after a callback.

## Overview

Use an appropriate status code to report your status when you complete a callback.

Note

Use a status code that is supported for the completion method you are calling.

| Method | Supported status codes |
|----|----|
| completePayment | STATUS_SUCCESS  STATUS_FAILURE  Use for Apple Pay API version 2 or earlier:  STATUS_INVALID_BILLING_POSTAL_ADDRESS  STATUS_INVALID_SHIPPING_POSTAL_ADDRESS  STATUS_INVALID_SHIPPING_CONTACT  STATUS_PIN_INCORRECT  STATUS_PIN_LOCKOUT  STATUS_PIN_REQUIRED |
| completeShippingContactSelection | STATUS_SUCCESS  STATUS_FAILURE  Use for Apple Pay API version 2 or earlier:  STATUS_INVALID_SHIPPING_POSTAL_ADDRESS |
| completeShippingMethodSelection | STATUS_SUCCESS  STATUS_FAILURE |

Apple Pay JS API supports customized errors in Apple Pay API version 3 and later. Use only STATUS_SUCCESS and STATUS_FAILURE for code using version 3. See ApplePayError for information on custom errors.

## Topics

### Status Code Constants

STATUS_FAILURE

The requested action failed.

STATUS_SUCCESS

The requested action succeeded.

STATUS_INVALID_BILLING_POSTAL_ADDRESS

The billing address is invalid.

STATUS_INVALID_SHIPPING_POSTAL_ADDRESS

The shipping address is invalid.

STATUS_INVALID_SHIPPING_CONTACT

The shipping contact information is invalid.

STATUS_PIN_INCORRECT

The PIN information is not valid.

STATUS_PIN_LOCKOUT

The maximum number of tries for a PIN has been reached and the user has been locked out.

STATUS_PIN_REQUIRED

The required PIN information was not provided.

## See Also

### Related Documentation

supportsVersion

Detects whether a web browser supports a particular Apple Pay version.

### Status and errors

ApplePayError

A customizable error type that you create to indicate problems with the address or contact information on an Apple Pay sheet.

ApplePayErrorCode

The error code that indicates whether an error on the payment sheet is for shipping or billing information, or for another kind of error.

ApplePayErrorContactField

Names of the fields in the shipping or billing contact information, used to locate errors in the payment sheet.

