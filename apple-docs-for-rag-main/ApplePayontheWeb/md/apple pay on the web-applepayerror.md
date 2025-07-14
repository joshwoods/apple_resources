

- Apple Pay on the Web
-  ApplePayError 

Class

# ApplePayError

A customizable error type that you create to indicate problems with the address or contact information on an Apple Pay sheet.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
interface ApplePayError
```

## Mentioned in 

Setting up the payment request API to accept Apple Pay

Choosing an API for Implementing Apple Pay on Your Website

Apple Pay on the Web Version 3 Release Notes

## Overview

When you determine that there’s a problem with an address or contact information on the payment sheet, you can use ApplePayError to create a customized error message. Apple Pay highlights the area with an error and displays your message, making it easier for users to correct errors.

Users must resolve any errors that you report on the Apple Pay sheet before they can finalize their transaction.

The details you provide in an Apple Pay error include:

- **code** — An error code that identifies the area of the error.

- **contactField** — The specific field on the payment sheet with the error.

- **message** — Your custom error message to display on the payment sheet.

For example, if you found an error in the postal code of the shipping address, create an ApplePayError with the custom message text `"ZIP Code is invalid"`, as follows:

```
```

Apple Pay highlights the postal code field and displays the message text on the payment sheet.

Note

ApplePayError requires Apple Pay API version 3 and later, and is only supported in Apple Pay JS API; it’s not available in the Payment Request API.

## Topics

### Creating an Apple Pay Error

ApplePayError

Creates an Apple Pay error object.

### Error Properties

code

The error code for this instance.

contactField

The field name that contains the error on the payment sheet.

message

A localized, user-facing string that describes the error.

## See Also

### Status and errors

ApplePayErrorCode

The error code that indicates whether an error on the payment sheet is for shipping or billing information, or for another kind of error.

ApplePayErrorContactField

Names of the fields in the shipping or billing contact information, used to locate errors in the payment sheet.

Apple Pay Status Codes

Codes used to report the status of an Apple Pay session after a callback.

