

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  paymentCouponCodeInvalidError(localizedDescription:) 

Type Method

# paymentCouponCodeInvalidError(localizedDescription:)

Returns an error object that indicates an invalid coupon.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOS

``` source
static func paymentCouponCodeInvalidError(localizedDescription: String? = nil) -> any Error
```

## Parameters 

`localizedDescription`  

A user-readable error as a localized string.

## Return Value

A new invalid coupon error.

## Discussion

Use this convenience method to create a payment error object instead of creating an NSError object yourself. This method indicates that the coupon code received from the Apple Pay sheet is invalid.

The error you provide and its optional message appear on the Apple Pay sheet. There’s limited available space to display messages, so keep your messages concise.

## See Also

### Providing error information

class func paymentBillingAddressInvalidError(withKey: String, localizedDescription: String?) -> any Error

Creates a billing address error with the supplied key and user-facing error message.

class func paymentContactInvalidError(withContactField: PKContactField, localizedDescription: String?) -> any Error

Creates a contact error with the supplied field and user-facing error message.

class func paymentShippingAddressInvalidError(withKey: String, localizedDescription: String?) -> any Error

Creates a shipping address error with the supplied key and user-facing error message.

class func paymentShippingAddressUnserviceableError(withLocalizedDescription: String?) -> any Error

Creates an error for an unserviceable address, with the supplied user-facing error message.

static func paymentCouponCodeExpiredError(localizedDescription: String?) -> any Error

Returns an error object that indicates an expired coupon.

