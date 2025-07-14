

- Apple Pay on the Web
-  ApplePayErrorContactField 

Enumeration

# ApplePayErrorContactField

Names of the fields in the shipping or billing contact information, used to locate errors in the payment sheet.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
enum ApplePayErrorContactField
```

## Overview

When shipping or billing contact information has an error, you use the error code values of either `"shippingContactInvalid"` or `"billingContactInvalid"` to indicate which one has the error. You use the contact field to indicate the exact field with the error. The corresponding field in the shipping or billing section of the payment sheet is highlighted.

Note that the remaining error codes, `"addressUnserviceable"` and `"unknown"`, do not require contact fields.

Use contact field values in the contactField property of an ApplePayError when you return errors in the completion functions, as shown in the following table.

Contact field values are available in all versions of the API except as stated in the table.

| Contact Field Value | Completion methods that support `"shippingContactInvalid"` error code | Completion methods that support `"billingContactInvalid"` error code |
|----|----|----|
| `"phoneNumber"` | completePayment |  |
| `"emailAddress"` | completePayment |  |
| `"name"` | completePayment | completePayment |
| `"phoneticName"`  (available starting in API version 3) | completePayment | completePayment |
| `"postalAddress"` | completeShippingContactSelection  completePayment | completePayment |
| `"addressLines"` | completePayment | completePayment |
| `"locality"` | completeShippingContactSelection  completePayment | completePayment |
| `"subLocality"` | completeShippingContactSelection  completePayment | completePayment |
| `"postalCode"` | completeShippingContactSelection  completePayment | completePayment |
| `"administrativeArea"` | completeShippingContactSelection  completePayment | completePayment |
| `"subAdministrativeArea"` | completeShippingContactSelection  completePayment | completePayment |
| `"country"` | completeShippingContactSelection  completePayment | completePayment |
| `"countryCode"` | completeShippingContactSelection  completePayment | completePayment |

## Topics

### Enumeration Cases

addressLines

administrativeArea

country

countryCode

emailAddress

locality

name

phoneNumber

phoneticName

postalAddress

postalCode

subAdministrativeArea

subLocality

## See Also

### Status and errors

ApplePayError

A customizable error type that you create to indicate problems with the address or contact information on an Apple Pay sheet.

ApplePayErrorCode

The error code that indicates whether an error on the payment sheet is for shipping or billing information, or for another kind of error.

Apple Pay Status Codes

Codes used to report the status of an Apple Pay session after a callback.

