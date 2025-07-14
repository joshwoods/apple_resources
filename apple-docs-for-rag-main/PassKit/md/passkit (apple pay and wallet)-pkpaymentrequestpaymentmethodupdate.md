

- PassKit (Apple Pay and Wallet)
-  PKPaymentRequestPaymentMethodUpdate 

Class

# PKPaymentRequestPaymentMethodUpdate

An object that updates the payment request after the payment method changes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class PKPaymentRequestPaymentMethodUpdate
```

## Overview

This is the handler for paymentAuthorizationController(_:didSelectPaymentMethod:handler:) and paymentAuthorizationViewController(_:didSelect:handler:). Update the summary items to reflect the change in payment method.

## Topics

### Creating a payment request update

init(errors: [any Error]?, paymentSummaryItems: [PKPaymentSummaryItem])

Creates a payment-method update with your specified payment summary items.

### Getting user errors

var errors: [any Error]!

An array of payment-method errors that the user must resolve.

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

class PKPaymentRequestShippingContactUpdate

An object that updates the payment request after the shipping contact information changes.

class PKPaymentRequestShippingMethodUpdate

An object that updates the payment request after the shipping method changed.

class PKPaymentRequestCouponCodeUpdate

An object that updates the payment request after the coupon code changes.

class PKPaymentRequestUpdate

The base class for updating the payment request after the user makes changes on the payment sheet.

