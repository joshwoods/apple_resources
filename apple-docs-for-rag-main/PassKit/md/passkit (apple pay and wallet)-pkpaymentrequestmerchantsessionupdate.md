

- PassKit (Apple Pay and Wallet)
-  PKPaymentRequestMerchantSessionUpdate 

Class

# PKPaymentRequestMerchantSessionUpdate

An object that updates a payment request with a merchant validation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+watchOS 7.0+

``` source
class PKPaymentRequestMerchantSessionUpdate
```

## Overview

This is the handler for paymentAuthorizationController(_:didRequestMerchantSessionUpdate:) and paymentAuthorizationViewController(_:didRequestMerchantSessionUpdate:).

## Topics

### Creating a merchant session update

init(status: PKPaymentAuthorizationStatus, merchantSession: PKPaymentMerchantSession?)

Creates a payment method update with the specified status and merchant session.

### Getting information for the merchant session update

var status: PKPaymentAuthorizationStatus

The current authorization status for the payment.

var session: PKPaymentMerchantSession?

An object that validates the identity of a merchant for the payment request.

class PKPaymentMerchantSession

An object that validates the identity of a merchant for a payment request.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Payment sheet updates

class PKPaymentRequestPaymentMethodUpdate

An object that updates the payment request after the payment method changes.

class PKPaymentRequestShippingContactUpdate

An object that updates the payment request after the shipping contact information changes.

class PKPaymentRequestShippingMethodUpdate

An object that updates the payment request after the shipping method changed.

class PKPaymentRequestCouponCodeUpdate

An object that updates the payment request after the coupon code changes.

class PKPaymentRequestUpdate

The base class for updating the payment request after the user makes changes on the payment sheet.

