

- PassKit (Apple Pay and Wallet)
-  PKPaymentRequestCouponCodeUpdate 

Class

# PKPaymentRequestCouponCodeUpdate

An object that updates the payment request after the coupon code changes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
class PKPaymentRequestCouponCodeUpdate
```

## Overview

This is the handler for paymentAuthorizationController(_:didChangeCouponCode:handler:) and paymentAuthorizationViewController(_:didChangeCouponCode:handler:).

Use this object to update the summary items to reflect the change in the coupon code.

Note

A coupon code error doesn’t block payment authorization.

## Topics

### Creating a payment coupon update object

init(errors: [any Error]?, paymentSummaryItems: [PKPaymentSummaryItem], shippingMethods: [PKShippingMethod])

Creates a payment coupon update with your specified payment summary items, errors, and shipping methods.

### Reading errors

var errors: [any Error]!

An array of errors for the coupon code that the user must resolve.

## Relationships

### Inherits From

- PKPaymentRequestUpdate

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Payment sheet updates

class PKPaymentRequestMerchantSessionUpdate

An object that updates a payment request with a merchant validation.

class PKPaymentRequestPaymentMethodUpdate

An object that updates the payment request after the payment method changes.

class PKPaymentRequestShippingContactUpdate

An object that updates the payment request after the shipping contact information changes.

class PKPaymentRequestShippingMethodUpdate

An object that updates the payment request after the shipping method changed.

class PKPaymentRequestUpdate

The base class for updating the payment request after the user makes changes on the payment sheet.

