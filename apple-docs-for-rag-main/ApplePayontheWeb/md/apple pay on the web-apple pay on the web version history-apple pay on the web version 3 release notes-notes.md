

- Apple Pay on the Web
- Apple Pay on the Web version history
-  Apple Pay on the Web Version 3 Release Notes 

Article

# Apple Pay on the Web Version 3 Release Notes

The version of Apple Pay available in macOS 10.13 and iOS 11.

## Overview

New features include:

- New error handling provided using ApplePayError.

- To support enhanced error handling, the number and type of arguments were changed for the following completion methods:

| Method | Argument for Version 3 | Arguments for Versions 1 and 2 |
|----|----|----|
| completePaymentMethodSelection | ApplePayPaymentMethodUpdate | completePaymentMethodSelection in Apple Pay JS API versions 1 and 2 |
| completeShippingContactSelection | ApplePayShippingContactUpdate | completeShippingContactSelection in Apple Pay JS version 1 and 2 |
| completeShippingMethodSelection | ApplePayShippingMethodUpdate | completeShippingMethodSelection in Apple Pay JS API version 1 and 2 |
| completePayment | ApplePayPaymentAuthorizationResult | completePayment in Apple Pay JS API version 1 and 2 |

- Support added for phonetic names in contact information, including `phoneticName` in ApplePayContactField; phoneticFamilyName and phoneticGivenName in ApplePayPaymentContact.

- Added a new property to ApplePayPaymentRequest called supportedCountries that lets you limit payments to cards from specific countries.

## See Also

### Apple Pay Version

Apple Pay on the Web Version 14 Release Notes

The version of Apple Pay available in macOS 13 and iOS 16.

Apple Pay on the Web Version 13 Release Notes

The version of Apple Pay available in macOS 12.3 and iOS 15.4.

Apple Pay on the Web Version 12 Release Notes

The version of Apple Pay available in macOS 12 and iOS 15.

Apple Pay on the Web Version 11 Release Notes

The version of Apple Pay available in macOS 11.5 and iOS 14.5.

Apple Pay on the Web Version 10 Release Notes

The version of Apple Pay available in macOS 11 and iOS 14.

Apple Pay on the Web Version 9 Release Notes

The version of Apple Pay available in macOS 10.15.6 and iOS 13.6.

Apple Pay on the Web Version 8 Release Notes

The version of Apple Pay available in macOS 10.15.1 and iOS 13.2.

Apple Pay on the Web Version 7 Release Notes

The version of Apple Pay available in macOS 10.14.6 and iOS 12.4.

Apple Pay on the Web Version 6 Release Notes

The version of Apple Pay available in macOS 10.14.4 and iOS 12.2.

Apple Pay on the Web Version 5 Release Notes

The version of Apple Pay available in macOS 10.14.2 and iOS 12.1.1.

Apple Pay on the Web Version 4 Release Notes

The version of Apple Pay available in macOS 10.14.1 and iOS 12.1.

Apple Pay on the Web Version 2 Release Notes

The version of Apple Pay available in macOS 10.12.1 and iOS 10.1.

Apple Pay on the Web Version 1 Release Notes

The version of Apple Pay available in macOS 10.12 and iOS 10.

