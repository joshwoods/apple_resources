

- Apple Pay on the Web
-  ApplePayErrorCode 

Enumeration

# ApplePayErrorCode

The error code that indicates whether an error on the payment sheet is for shipping or billing information, or for another kind of error.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
enum ApplePayErrorCode
```

## Overview

Use the following error codes in the code property of ApplePayError:

`"shippingContactInvalid"`  
The code that indicates that the shipping address or contact information is invalid or missing.

Use with contactField.

`"billingContactInvalid"`  
The code that indicates that the billing address information is invalid or missing.

Use with contactField.

`"addressUnserviceable"`  
The code that indicates that the merchant can’t provide service to the shipping address (for example, can’t deliver to a P.O. Box).

`"couponCodeInvalid"`  
The code that indicates an invalid coupon.

`"couponCodeExpired"`  
The code that indicates an expired coupon.

`"unknown"`  
The code that indicates an unknown but nonfatal error occurred during payment processing. The user can attempt authorization again.

## Topics

### Enumeration Cases

addressUnserviceable

billingContactInvalid

couponCodeExpired

couponCodeInvalid

shippingContactInvalid

unknown

## See Also

### Status and errors

ApplePayError

A customizable error type that you create to indicate problems with the address or contact information on an Apple Pay sheet.

ApplePayErrorContactField

Names of the fields in the shipping or billing contact information, used to locate errors in the payment sheet.

Apple Pay Status Codes

Codes used to report the status of an Apple Pay session after a callback.

