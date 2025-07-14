

- PassKit (Apple Pay and Wallet)
-  PKPaymentRequestShippingContactUpdate 

Class

# PKPaymentRequestShippingContactUpdate

An object that updates the payment request after the shipping contact information changes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class PKPaymentRequestShippingContactUpdate
```

## Overview

This is the handler for paymentAuthorizationController(_:didSelectShippingContact:handler:) and paymentAuthorizationViewController(_:didSelectShippingContact:handler:).

Use this object to update the available shipping methods and, if the user has selected a shipping method, the current shipping cost.

## Topics

### Creating a shipping contact update

init(errors: [any Error]?, paymentSummaryItems: [PKPaymentSummaryItem], shippingMethods: [PKShippingMethod])

Creates a shipping contact update with your specified payment summary items and shipping methods.

### Updating user errors and shipping methods

var errors: [any Error]!

An array of shipping contact information errors that the user must resolve.

var shippingMethods: [PKShippingMethod]

An array of shipping methods.

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

class PKPaymentRequestShippingMethodUpdate

An object that updates the payment request after the shipping method changed.

class PKPaymentRequestCouponCodeUpdate

An object that updates the payment request after the coupon code changes.

class PKPaymentRequestUpdate

The base class for updating the payment request after the user makes changes on the payment sheet.

