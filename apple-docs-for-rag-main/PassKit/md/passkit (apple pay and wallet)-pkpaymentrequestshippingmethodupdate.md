

- PassKit (Apple Pay and Wallet)
-  PKPaymentRequestShippingMethodUpdate 

Class

# PKPaymentRequestShippingMethodUpdate

An object that updates the payment request after the shipping method changed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class PKPaymentRequestShippingMethodUpdate
```

## Overview

This is the handler for paymentAuthorizationController(_:didSelectShippingMethod:handler:) and paymentAuthorizationViewController(_:didSelect:handler:).

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

class PKPaymentRequestCouponCodeUpdate

An object that updates the payment request after the coupon code changes.

class PKPaymentRequestUpdate

The base class for updating the payment request after the user makes changes on the payment sheet.

