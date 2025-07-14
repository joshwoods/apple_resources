

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  paymentContactInvalidError(withContactField:localizedDescription:) 

Type Method

# paymentContactInvalidError(withContactField:localizedDescription:)

Creates a contact error with the supplied field and user-facing error message.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class func paymentContactInvalidError(
    withContactField field: PKContactField,
    localizedDescription: String?
) -> any Error
```

## Parameters 

`field`  

A value from PKContactField that indicates which part of the contact information has an error.

`localizedDescription`  

Optional. Provide a localized, user-facing error message string to help the user resolve the error.

## Discussion

You can use this convenience method to create a payment error object instead of creating an NSError object yourself. This method indicates an error in the contact information that is received from an Apple Pay sheet.

The error you provide and its optional message appear on the Apple Pay sheet. The available space to display messages is limited, so you should keep your messages concise.

## See Also

### Providing error information

class func paymentBillingAddressInvalidError(withKey: String, localizedDescription: String?) -> any Error

Creates a billing address error with the supplied key and user-facing error message.

class func paymentShippingAddressInvalidError(withKey: String, localizedDescription: String?) -> any Error

Creates a shipping address error with the supplied key and user-facing error message.

class func paymentShippingAddressUnserviceableError(withLocalizedDescription: String?) -> any Error

Creates an error for an unserviceable address, with the supplied user-facing error message.

static func paymentCouponCodeInvalidError(localizedDescription: String?) -> any Error

Returns an error object that indicates an invalid coupon.

static func paymentCouponCodeExpiredError(localizedDescription: String?) -> any Error

Returns an error object that indicates an expired coupon.

